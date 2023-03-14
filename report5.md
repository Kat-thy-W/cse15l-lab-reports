# Lab Report 5 Grading Script
## Information of the Grading Script lab
- Grading Script is a bash script that work with TestListExamples.java to give a score on students' ListExamples submission
- TestListExamples.java is a Junit test file, my TestListExample.java has total of four test, two of which test the merge method and the other two test the filter method. Since the focus of this lab is on bash script, details on the TestListExamples.java are omitted.
- the Junit library path in based on windows system, the mac version is `CPATH='.:../lib/hamcrest-core-1.3.jar:../lib/junit-4.13.2.jar`
## Improvement
- Work on nested file
- Return score as a fraction instead of pass/failed

## Code of the Grading Script
```
CPATH='.;../lib/hamcrest-core-1.3.jar;../lib/junit-4.13.2.jar'

rm -rf student-submission
git clone $1 student-submission
echo 'Finished cloning'

CFILE=`find -name "ListExamples.java"`
# Search for file in case of file is nested

if [[ $CFILE != "" ]]
then
        echo "ListExamples.java found"
else
        echo "ListExamples.java is missing"
        exit 1
fi

cp *.java ./student-submission
cp $CFILE ./student-submission
# Move all files to the student-submission for neatness

cd student-submission

set +e 
# set +e turn auto-exit off

javac -cp $CPATH *.java > compile.txt

if [[ $? -eq 0 ]]
then
        echo "Files compiled"
else
        echo "Compilation error, Your Score is 0"
        cat compile.txt
        exit
fi

java -cp $CPATH org.junit.runner.JUnitCore TestListExamples > results.txt
FAILURES=`grep -c FAILURES!!! results.txt`

if [[ $FAILURES -eq 0 ]]
then
        RESULTLINE=`grep -w "OK " results.txt`
        TESTCOUNT=${RESULTLINE:4:1}
        echo "Your Score is: $TESTCOUNT/$TESTCOUNT"
else
        RESULTLINE=`grep -w "run:" results.txt`
        PASSED=${RESULTLINE:25:1}
        TOTAL=${RESULTLINE:11:1}
        echo "Your Score is: $PASSED/$TOTAL"
fi

echo "JUitn out was: "
cat results.txt
```
## Limitation
- This Grading Script score function works only if there are less than or equal to 9 tests, for more tests, some code needed to be changed
## Some result of the Grade Script
### Test 1

- Student Submission [https://github.com/ucsd-cse15l-f22/list-methods-lab3](https://github.com/ucsd-cse15l-f22/list-methods-lab3)
- Submission Note: has starter cost
- Expected Behavior: Complie but fail some of the test, return a score base on test passed.
- Result:

![image](https://user-images.githubusercontent.com/115119572/224884932-f04e3c38-4411-4fb2-8a32-8231e9cddabf.png)
### Test 2
- Student Submission [https://github.com/ucsd-cse15l-f22/list-methods-corrected](https://github.com/ucsd-cse15l-f22/list-methods-corrected)
- Submission Note: correct
- Expected Behavior: Complie and pass all test, return a score.
- Result:

![image](https://user-images.githubusercontent.com/115119572/224885441-aba34c63-d061-4a3b-a5f2-109276394b7e.png)
### Test 3
- Student Submission [https://github.com/ucsd-cse15l-f22/list-methods-compile-error](https://github.com/ucsd-cse15l-f22/list-methods-compile-error)
- Submission Note: Compile error
- Expected Behavior: Complie error and exit test. Return a score of 0.
- Result:

![image](https://user-images.githubusercontent.com/115119572/224885846-ccc407f9-fb30-49e6-986f-59855f15405c.png)
### Test 4
- Student Submission [https://github.com/ucsd-cse15l-f22/list-methods-nested](https://github.com/ucsd-cse15l-f22/list-methods-nested)
- Submission Note: correct code, but the ListExamples.java is nested in another file
- Expected Behavior: Complie and pass all test, return a score.
- Result:

![image](https://user-images.githubusercontent.com/115119572/224886271-91ccc661-68dd-4c2c-83fc-ae83e875fc41.png)




