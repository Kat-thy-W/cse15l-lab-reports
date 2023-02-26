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
comment in terminal `cd lab7/` 
2. Compile java files with Junit \
Key Pressed: `javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java` 
3. Run Junit test \
Key Pressed: `java -cp `.:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests`
![image](https://user-images.githubusercontent.com/115119572/221404858-df0b7696-927a-4bb3-98ad-19572c846b09.png)
