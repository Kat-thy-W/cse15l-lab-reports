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


