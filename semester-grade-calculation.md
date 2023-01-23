### Part 1
Write a function which takes in a `student` object as shown and adds an appropriate grade for the given `semester`. 

Here is how grades are alloted:
```
Grade A - avg score greater then 90
Grade B - avg score greater than 80
Grade C - avg score greater than 70
Grade D - avg score greater than 60
Grade E - avg score greater than 50
Grade F - otherwise
```

For e.g. for the following student, if we want to calculate grade of semester 2
```js
function addGrade(student, semester) {
  // your code here
}

let student1 = { name: 'Akshat', scores: [[90, 100], [80, 80], [80, 100], [60, 60]] };

addGrade(student1, 2); // since the semester value is 2 the scores will be 100, 80, 100 and 60 so adding them gives 340. 
// So the average value will be 85. And Hence the grade is `B`. So we will add the property `semeseter2_grade` with the value `B`.

console.log(student1); // should print{ name: 'Akshat', scores: [[90, 100], [80, 80], [80, 100], [60, 60]], semeseter2_grade: 'B' };
```


### Part 2

You are given several students' score for two different semesters.

Calculate the grade for the student for the given semester and add it as a property like 'semester1_grade' or `semester2_grade` based on the given semester value. Make use of the function you wrote in previous exercise.

``` js

let students = [
  { name: 'Vivek', scores: [[70, 60], [90, 100], [60, 80], [91, 59]] },
  { name: 'Akshat', scores: [[90, 100], [80, 80], [80, 100], [60, 60]] },
  { name: 'Arnav', scores: [[70, 40], [60, 60], [90, 100], [90, 90]] },
  { name: 'Pawan', scores: [[80, 80], [90, 60], [90, 40], [70, 80]] }
];

addGrades(students, 1); // should add `semester1_grade` property to each student
```
