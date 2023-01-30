# Lab Report 2
------
## Part 1: StringServer
---
- Code for StringServer

![image](https://user-images.githubusercontent.com/115119572/215466752-d0837da1-1f8a-41e5-a011-efab28677ab1.png)

- Before Server generate a link and before we can add message on the server, these methods are called:
  - String Server contains the main method, which call the server.start method.
  - Inside the server.start method, and new instance of StringHandler is created.
- Add Message: hi
  - Which methods:
    - the handleRequest method under class StringHandler runed
  - Arguments: 
    - the url itself
  - values: 
    - http://localhost:3672/add-message?s=hi 
  - field in class changed:
    - the Arraylist ls inside of StringHandler class has a new string "hi" in index 0
![image](https://user-images.githubusercontent.com/115119572/215461643-bc9e504a-4daa-4e10-b560-57107265ea53.png)
- Add Message: who is there
  - Which methods:
    - the handleRequest method under class StringHandler runed
  - Arguments: 
    - the url itself
  - values: 
    - http://localhost:3672/add-message?s=who%20is%20there?
  - field in class changed:
    - the Arraylist ls inside of StringHandler class has a new string "who is there" on index 2 
![image](https://user-images.githubusercontent.com/115119572/215466966-add1c9e9-215e-46de-89e4-095eb73457ac.png)
-----
## Part2: Lab 3 Bugs: List Example
- relavent code for both tests and an implemetation of StringChecker
````
public class ListTests {
    public class ContainsCat implements StringChecker{
        @Override
        public boolean checkString(String s){
            if(s.contains("CAT") || s.contains("cat") || s.contains("Cat") ){
                return true;}
            return false;
        }
    }
````
- Failure inducing input (inside of the ListTest class)
````
    @Test
    public void testFilter1(){
        ArrayList<String> inputList = new ArrayList<>(List.of("cat", "Dog", "Kitty Cat"));
        String[] ExpectedOutput = new String[]{"cat", "Kitty Cat"};
        List<String> actualOutput = ListExamples.filter(inputList, new ContainsCat());
        assertEquals(2, actualOutput.size());
        String[] output = new String[] {actualOutput.get(0), actualOutput.get(1)};
        assertArrayEquals(ExpectedOutput, output)
````
- input that does not induce failure(inside of the ListTest class)
````
    @Test
    public void testFilter2(){
        ArrayList<String> inputList = new ArrayList<>(List.of("kitty cat", "Dog", "kitty"));
        String[] ExpectedOutput = new String[]{"kitty cat"};
        List<String> actualOutput = ListExamples.filter(inputList, new ContainsCat());
        String[] output = new String[] {actualOutput.get(0)};
        assertArrayEquals(ExpectedOutput, output);
    }
````
- Symptom: 
![image](https://user-images.githubusercontent.com/115119572/215474288-fe3895c2-78ee-42e9-948f-c3a5a3cde620.png)

- bug (inside of the ListExample class):

  - before: 
  ````
    static List<String> filter(List<String> list, StringChecker sc) {
    List<String> result = new ArrayList<>();
    for(String s: list) {
      if(sc.checkString(s)) {
        result.add(0, s);
      }
    }
    return result;
  }
  ````
  - after
  ````
    static List<String> filter(List<String> list, StringChecker sc) {
    List<String> result = new ArrayList<>();
    for(String s: list) {
      if(sc.checkString(s)) {
        result.add(s);
        //previously the method always add the new string from the front, which mess up the order
        //the after version will add string to the back of the array, which keep the order
      }
    }
    return result;
  }
  ````
 The only issue of the filter method in ListExample is the order of the filter result is reverted becuase the result.add method try to always add from the front. We can need to revise the method to add to the end

-----
## Part 3: Things I Learned
I would like to use a list to show some of the times I learn these two weeks
- I learn how to create a code block in Markdown
- I learn how to open git bash in visual studio code. Prior to that, I was using git bash on the git bash terminal, which was casuing me a lots of trauble
- I gain some understanding on how url and server works
- I build a very simple server, and understand what path and quary means
- I learn how to commit and push a code, then fork it and run it on a remote server
