# java-interview-test
Java problem to solve before interviews.

## Setup
### IntelliJ

- Clone this repository.
- Get IntelliJ community edition from [here](https://www.jetbrains.com/idea/download/)
- Start IntelliJ, choose "Import Project":
<a href="http://i.imgur.com/Llah7Ss.png"><img src="http://i.imgur.com/Llah7Ss.png" width="48"></a>
- Select the `direct-reports` folder:
<a href="http://i.imgur.com/fOI6WHO.png"><img src="http://i.imgur.com/fOI6WHO.png" width="48"></a>
- Choose "Import project from external model", and "Maven":
<a href="http://i.imgur.com/fHx1Oo9.png"><img src="http://i.imgur.com/fHx1Oo9.png" width="48"></a>
- Leave everything and click "Next" on the next screen:
<a href="http://i.imgur.com/nqrvBtY.png"><img src="http://i.imgur.com/nqrvBtY.png" width="48"></a>
- Leave everything and click "Next" on the next screen:
<a href="http://i.imgur.com/0s2U2sM.png"><img src="http://i.imgur.com/0s2U2sM.png" width="48"></a>
- Make sure to choose Java 8 (or add it):
<a href="http://i.imgur.com/5aLmYO8.png"><img src="http://i.imgur.com/5aLmYO8.png" width="48"></a>
- Click "Finish" on the last screen:
<a href="http://i.imgur.com/0vPbpuB.png"><img src="http://i.imgur.com/0vPbpuB.png" width="48"></a>

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
