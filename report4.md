# Command Line in Remote Server
## 1. Log into ieng6
Key pressed: `<up><enter>`  \
The `ssh cs15lwi23ala@ieng6.ucsd.edu` command was 1 up in the search history, so I used up arrow to access it.
![image](https://user-images.githubusercontent.com/115119572/221403747-18d1c1b8-8f8d-4dd7-8256-1b593d8bc82d.png)
## 2. Use ssh to clone Repository
1. Create a fork of the lab 7 repository
![image](https://user-images.githubusercontent.com/115119572/221404240-0f934039-aaaa-4a07-b1bf-48080704885f.png)
2. Copy ssh link from forked copy
![image](https://user-images.githubusercontent.com/115119572/221404432-be849d21-0a62-4d49-bd74-bf0b8eb45ffe.png)
3. Clone to ieng6 server \
Key pressed: `ssh clone <ctrl> <v> <enter>` \
the `git clone git@github.com:Kat-thy-W/lab7.git` is passed into system
![image](https://user-images.githubusercontent.com/115119572/221404003-03250457-cc9d-49fd-93f4-8be3e332d3c7.png)
## 3. Run the tests, demonstrating that they fail
1. Change to lab 7 directory \
Key Pressed: `cd l<tab> <enter>` \
Command in terminal `cd lab7/` 
2. Compile java files with Junit \
Key Pressed: `javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java` 
3. Run Junit test \
Key Pressed: `java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests` \
result: one test fail.
![image](https://user-images.githubusercontent.com/115119572/221404858-df0b7696-927a-4bb3-98ad-19572c846b09.png)
## 4.Edit the code file to fix the failing test
1. Use nano to edit ListExamples.java \
Key pressed: `Lis<tab>.j<tab><enter>` \
Command in terminal: `nano ListExamples.java`
![image](https://user-images.githubusercontent.com/115119572/221405200-7cc5ab47-564d-44cc-9790-d4928a703a22.png)
2. Use keyboard arrows navigate to the error, change increment of index1 to increment of index2, save changes and exit nano editor \
Key Pressed: after editing errors, `<ctrl> <o> <enter> <Ctrl> <x>` \
![image](https://user-images.githubusercontent.com/115119572/221405346-d66b45a1-7810-4044-aeae-b2c310686132.png)
## 5. Run the tests, demonstrating that they now succeed
1. Recompile files \
Key pressed: `<up><up><up><enter>` \
Command in system: `javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java` command was 3 up in the search history, so I used up arrow to access it.
2. Run the test 
3. Key pressed: `<up><up><up><enter>` \
Command in system: `java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests` command was 3 up in the search history, so I used up arrow to access it. \
Result
![image](https://user-images.githubusercontent.com/115119572/221405685-17011775-dc75-4af8-8fdf-f080b228b304.png)
## 6. Commit and push the resulting change to my Github account
1. Add file \
Key Pressed: `git add Lis<tab>.j<tab><enter>` \
Command in system: `git add ListExamples.java`
2. Commit changes \
Key Preesed: `git commit -m "changed"` \
![image](https://user-images.githubusercontent.com/115119572/221406234-b85b4b1a-ab6e-4fab-8063-6abcfb128643.png)
3. Push new Commit to github \
Key Pressed: ` git push` \
![image](https://user-images.githubusercontent.com/115119572/221406311-550326f7-a140-4cb6-9b76-070baee24efa.png)


