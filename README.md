# java-interview-test
Java problem to solve before interviews.

## Setup
### IntelliJ

- Clone this repository.
- Get IntelliJ community edition from [here](https://www.jetbrains.com/idea/download/)
- Start IntelliJ, choose "Import Project":
![screen 1](http://i.imgur.com/Llah7Ss.png "screen 1")
- Select the `direct-reports` folder:
![screen 2](http://i.imgur.com/fOI6WHO.png "screen 2")
- Choose "Import project from external model", and "Maven":
![screen 3](http://i.imgur.com/fHx1Oo9.png "screen 3")
- Leave everything and click "Next" on the next screen:
![screen 4](http://i.imgur.com/nqrvBtY.png "screen 4")
- Leave everything and click "Next" on the next screen:
![screen 5](http://i.imgur.com/0s2U2sM.png "screen 5")
- Make sure to choose Java 8 (or add it):
![screen 6](http://i.imgur.com/5aLmYO8.png "screen 6")
- Click "Finish" on the last screen:
![screen 7](http://i.imgur.com/0vPbpuB.png "screen 7")

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
For Example Only:
Jan Levinson
      |
      |__ Michael Scott
      |         |
      |         |__ Jim Halpert
      |         |__ Pamela Beasley
      |
      |__ Toby Flenderson
```

- Add your code to the `PersonToPersonTreeNodeConverter`.`generateTree()` method.
![do exercise](http://i.imgur.com/7QAAf4S.png "do exercise")
- Run the junit test in `PersonToPersonTreeNodeConverterTest`.
![run test](http://i.imgur.com/y46jqNe.png "run test")
- Repeat until test passes.
- Zip the project folder and email it to us.
