# java-interview-test
Java problem to solve before interviews.

## Setup
### IntelliJ

- Clone the repository. 
- Get IntelliJ community edition from [here](https://www.jetbrains.com/idea/download/)
- In IntelliJ add as a new project 'from existing sources'.
![file menu image](http://i.imgur.com/1iL8qMb.png "file menu screenshot")
- If asked to overwrite things, just say 'yes'.

### Any Other IDE

- Clone the repository.
- Delete any .iml files or .idea folders if your IDE does not like them.
- You may need to add `junit` to the classpath of the `direct-reports` project/module.


## Solving The Test

Given an array of employees:
```
Name: Jan Levinson 
Manager: null
 
Name: Michael Scott
Manager: Jan Levinson
 
Name: Toby Flenderson
Manager: Jan Levinson
 
Name: Jim Halpert
Manager: Michael Scott
 
Name: Pamela Beasley
Manager: Michael Scott
```
Return a single tree node representing the company org chart:
```
Jan Levinson
      |
      |__ Michael Scott
      |         |
      |         |__ Jim Halpert
      |         |__ Pamela Beasley 
      |
      |__ Toby Flenderson 
```

- Add your code to the `PersonToPersonTreeNodeConverter`.`generateTree` method.
- Run the junit test in `PersonToPersonTreeNodeConverterTest`.
- Repeat until test passes.
- Zip the project folder and email it to us.