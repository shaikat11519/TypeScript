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
- _number_
- _string_
- _boolean_
- _void_
- _undefined_
- _null_

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
> _User Define Type 

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

### Array Data Type
> Multiple Type Of Array

> Single Type of Array
```typeScript

let studentNames: string[];
// let studentNames Array<string>

studentNames = ["Shaikat", "Alif", "Showan", "Suzon"];

console.log(studentNames[1]);

// Multiple Type Of Array

let studentNameAndAge: (number | string) [];
studentNameAndAge = ["Shaikat", "Alif", "Showan", 21, 23, 24];

console.log(studentNameAndAge[3]);
console.log("Students Sort List: "+ studentNameAndAge.sort());

studentNameAndAge.push("Ashiq");
console.log("Student insert at last index: "+ studentNameAndAge);

studentNameAndAge.pop();
console.log("Student Drop from at last index: "+ studentNameAndAge);

studentNameAndAge.shift();
console.log("Student Drop at First index: "+ studentNameAndAge);

studentNameAndAge.unshift("chomok");
console.log("Student Insert at First index: "+ studentNameAndAge);
```

### Tuple Data Type
> Tuple Type | Mixed data type

```typeScript
let studentNameAndAge: [string, number];
studentNameAndAge = ["Shaikat", 41];

studentNameAndAge.push("Alif", 21);
console.log(studentNameAndAge);
```

### Enum Data Type
> Enum Type: no duplicate data, helps to store constants

- _numeric_
- _string_
- _hetergenous_


> Numeric Enum
```typeScript
enum RequestType{
    readData,
    //readData = 1,
    saveData,
    deleteData,
}

console.log(RequestType);
console.log(RequestType.readData);
console.log(RequestType["readData"]);
```

> String Enum
```typeScript
enum RequestType2{
    readData = "READ_DATA",
    deleteData = "DELETE_DATA",
}

console.log(RequestType2.deleteData);
console.log(RequestType2["deleteData"]);
```

> Hetergenous Enum
```typeScript
enum RequestType3{
    readData = "READ_DATA",
    deleteData = "DELETE_DATA",
    roll = 1163
}
console.log(RequestType3.deleteData);
console.log(RequestType3.roll);
```

### Any type
-> user input values

```js
let userName: any;

userName = "Shaikat";
userName = 1163;
userName = true;
userName = [41, 36];

 // another Example
 let password: any;
 let passwords: any[];
 ```

