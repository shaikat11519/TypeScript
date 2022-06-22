## TypeScript

#### What is TypeScript?

- In a simple words, Types + JavaScript = TypeScript
- It is a superset of JS
- developed and maintained by Microsoft

#### Why TypeScript?

- JS Check types in run time while typescript add static typing to JS so we can handle errors before running the program.
- increase readability and code quality
- popular JS libraray Angular use TypeScript.
- It can be used in both: client and server side.
- Intellisense IDE Support while coding: code completion, content assist and code hinting


### Built in data type
- number, 
- string,
- boolean, 
- void, 
- undefined, 
- null

```typescript
let studentId: number;
let studentFirst: string;
let studentLast: string;
let studentName: string;
let isStudent: boolean;

studentId = 14141;
studentFirst = "Ashikujjaman";
studentLast = " Shaikat";
isStudent = true;

studentName = studentFirst.concat(studentLast);

console.log("Split:" + studentName.split(" "));
console.log("UperCase:" + studentName.toUpperCase());
console.log("LowerCase:" + studentName.toLowerCase());

console.log(`ID: ${studentId}, Name: ${studentName}, is Student: ${isStudent}`);
```

### Union Data Type
> User Define Type 

```typeScript
let studentId: string | number;

studentId = "171-15-1163";
studentId = 1163;

function displayStudentId(studentId: string | number){
    console.log(studentId);
}

displayStudentId(1163);
displayStudentId("171-15-1163");
```
