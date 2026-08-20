# MongoDB-queires

Windows PowerShell
Copyright (C) Microsoft Corporation. All rights reserved.

Install the latest PowerShell for new features and improvements! https://aka.ms/PSWindows

PS C:\Users\91778> mongosh 27017
Current Mongosh Log ID: 6a869bf4a152a947acfa4213
Connecting to:          mongodb://127.0.0.1:27017/27017?directConnection=true&serverSelectionTimeoutMS=2000&appName=mongosh+2.4.0
Using MongoDB:          8.3.8
Using Mongosh:          2.4.0
mongosh 2.10.0 is available for download: https://www.mongodb.com/try/download/shell

For mongosh info see: https://www.mongodb.com/docs/mongodb-shell/

------
   The server generated these startup warnings when booting
   2026-08-17T10:02:10.928+05:30: Access control is not enabled for the database. Read and write access to data and configuration is unrestricted
------

27017> use collegeDB
switched to db collegeDB
collegeDB> db.students.insertMany([{
... name : "Arav",
... age: 21,
... dept: "CSE",
... marks: 90,
... city: "Hyderabad",
... skills: ["python", "mongodb"],
... fees: {total: 50000, paid: 30000}
... },
... {
... name : "Divya",
... age: 22,
... dept: "ECE",
... marks: 72,
... skills: ["c", "verilog"],
... city: "Chennai",
... fees: {total: 45000, paid: 45000}
... },
... {
... name:"Kabir",
... age: 20,
... dept: "CSE",
... marks: 91,
... skills:["java","sql","mongodb"],
... city:"Hyderabad",
... fees:{total:50000,paid:50000}
... },
... {
... name:"Meera",
... age:23,
... dept:"MECH",
... marks:64,
... skills:["autocad"],
... city:"Pune",
... fees:{total:40000,paid:20000}
... },
... {
... name:"Rohan",
... age:21,
... dept:"CSE",
... marks:78,
... skills:["python","sql"],
... city:"Chennai",
... fees:{total:50000,paid:40000}
... },
... {
... name:"Sana",
... age:22,
... dept:"ECE"
... marks:88,
Uncaught:
SyntaxError: Unexpected token, expected "," (50:0)

  48 | age:22,
  49 | dept:"ECE"
> 50 | marks:88,
     | ^
  51 |

collegeDB> db.students.insertMany([{ name : "Arav", age: 21, dept: "CSE", marks: 90, city: "Hyderabad", skills: ["python", "mongodb"], fees: {total: 50000, paid: 30000} }, { name : "Divya", age: 22, dept: "ECE", marks: 72, skills: ["c", "verilog"], city: "Chennai", fees: {total: 45000, paid: 45000} }, { name:"Kabir", age: 20, dept: "CSE", marks: 91, skills:["java","sql","mongodb"], city:"Hyderabad", fees:{total:50000,paid:50000} }, { name:"Meera", age:23, dept:"MECH", marks:64, skills:["autocad"], city:"Pune", fees:{total:40000,paid:20000} }, { name:"Rohan", age:21, dept:"CSE", marks:78, skills:["python","sql"], city:"Chennai", fees:{total:50000,paid:40000} }, { name:"Sana", age:22, dept:"ECE" marks:88,skills:["python","matlab"],
Uncaught:
SyntaxError: Unexpected token, expected "," (1:692)

> 1 | db.students.insertMany([{ name : "Arav", age: 21, dept: "CSE", marks: 90, city: "Hyderabad", skills: ["python", "mongodb"], fees: {total: 50000, paid: 30000} }, { name : "Divya", age: 22, dept: "ECE", marks: 72, skills: ["c", "verilog"], city: "Chennai", fees: {total: 45000, paid: 45000} }, { name:"Kabir", age: 20, dept: "CSE", marks: 91, skills:["java","sql","mongodb"], city:"Hyderabad", fees:{total:50000,paid:50000} }, { name:"Meera", age:23, dept:"MECH", marks:64, skills:["autocad"], city:"Pune", fees:{total:40000,paid:20000} }, { name:"Rohan", age:21, dept:"CSE", marks:78, skills:["python","sql"], city:"Chennai", fees:{total:50000,paid:40000} }, { name:"Sana", age:22, dept:"ECE" marks:88,skills:["python","matlab"],
    |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     ^
  2 |

collegeDB> db.students.insertMany([{ name : "Arav", age: 21, dept: "CSE", marks: 90, city: "Hyderabad", skills: ["python", "mongodb"], fees: {total: 50000, paid: 30000} }, { name : "Divya", age: 22, dept: "ECE", marks: 72, skills: ["c", "verilog"], city: "Chennai", fees: {total: 45000, paid: 45000} }, { name:"Kabir", age: 20, dept: "CSE", marks: 91, skills:["java","sql","mongodb"], city:"Hyderabad", fees:{total:50000,paid:50000} }, { name:"Meera", age:23, dept:"MECH", marks:64, skills:["autocad"], city:"Pune", fees:{total:40000,paid:20000} }, { name:"Rohan", age:21, dept:"CSE", marks:78, skills:["python","sql"], city:"Chennai", fees:{total:50000,paid:40000} }, { name:"Sana", age:22, dept:"ECE" marks:88,skills:["python","matlab"],city:"Hyderabad",fees:{total:45000,paid:45000}}])
Uncaught:
SyntaxError: Unexpected token, expected "," (1:692)

> 1 | db.students.insertMany([{ name : "Arav", age: 21, dept: "CSE", marks: 90, city: "Hyderabad", skills: ["python", "mongodb"], fees: {total: 50000, paid: 30000} }, { name : "Divya", age: 22, dept: "ECE", marks: 72, skills: ["c", "verilog"], city: "Chennai", fees: {total: 45000, paid: 45000} }, { name:"Kabir", age: 20, dept: "CSE", marks: 91, skills:["java","sql","mongodb"], city:"Hyderabad", fees:{total:50000,paid:50000} }, { name:"Meera", age:23, dept:"MECH", marks:64, skills:["autocad"], city:"Pune", fees:{total:40000,paid:20000} }, { name:"Rohan", age:21, dept:"CSE", marks:78, skills:["python","sql"], city:"Chennai", fees:{total:50000,paid:40000} }, { name:"Sana", age:22, dept:"ECE" marks:88,skills:["python","matlab"],city:"Hyderabad",fees:{total:45000,paid:45000}}])
    |                                                                                                                                collegeDB> db.students.insertMany([{ name : "Arav", age: 21, dept: "CSE", marks: 90, city: "Hyderabad", skills: ["python", "mongodb"], fees: {total: 50000, paid: 30000} }, { name : "Divya", age: 22, dept: "ECE", marks: 72, skills: ["c", "verilog"], city: "Chennai", fees: {total: 45000, paid: 45000} }, { name:"Kabir", age: 20, dept: "CSE", marks: 91, skills:["java","sql","mongodb"], city:"Hyderabad", fees:{total:50000,paid:50000} }, { name:"Meera", age:23, dept:"MECH", marks:64, skills:["autocad"], city:"Pune", fees:{total:40000,paid:20000} }, { name:"Rohan", age:21, dept:"CSE", marks:78, skills:["python","sql"], city:"Chennai", fees:{total:50000,paid:40000} }, { name:"Sana", age:22, dept:"ECE",marks:88,skills:["python","matlab"],city:"Hyderabad",fees:{total:45000,paid:45000}}])
{
  acknowledged: true,
  insertedIds: {
    '0': ObjectId('6a869eb6a152a947acfa4214'),
    '1': ObjectId('6a869eb6a152a947acfa4215'),
    '2': ObjectId('6a869eb6a152a947acfa4216'),
    '3': ObjectId('6a869eb6a152a947acfa4217'),
    '4': ObjectId('6a869eb6a152a947acfa4218'),
    '5': ObjectId('6a869eb6a152a947acfa4219')
  }
}
collegeDB> db.departments.inserMany([
... {
... code:"CSE", fullName: "ComputerScience", hod: "Dr.Rao"}
... {code:"ECE", fullName: "Electronics", hod:"Dr.Iyer"}
Uncaught:
SyntaxError: Unexpected token, expected "," (4:0)

  2 | {
  3 | code:"CSE", fullName: "ComputerScience", hod: "Dr.Rao"}
> 4 | {code:"ECE", fullName: "Electronics", hod:"Dr.Iyer"}
    | ^
  5 |

collegeDB> db.departments.inserMany([ { code:"CSE", fullName: "ComputerScience", hod: "Dr.Rao"} {code:"ECE", fullName: "Electronics", hod:"Dr.Iyer"},{code:"MECH", fullName: "Mechanical", hod:"Dr.Khan"}])
Uncaught:
SyntaxError: Unexpected token, expected "," (1:85)

> 1 | db.departments.inserMany([ { code:"CSE", fullName: "ComputerScience", hod: "Dr.Rao"} {code:"ECE", fullName: "Electronics", hod:"Dr.Iyer"},{code:"MECH", fullName: "Mechanical", hod:"Dr.Khan"}])
    |                                                                                      ^
  2 |

collegeDB> db.departments.inserMany([ { code:"CSE", fullName: "ComputerScience", hod: "Dr.Rao"},{code:"ECE", fullName: "Electronics", hod:"Dr.Iyer"},{code:"MECH", fullName: "Mechanical", hod:"Dr.Khan"}])
TypeError: db.departments.inserMany is not a function
collegeDB> db.departments.insertMany([ { code:"CSE", fullName: "ComputerScience", hod: "Dr.Rao"},{code:"ECE", fullName: "Electronics", hod:"Dr.Iyer"},{code:"MECH", fullName: "Mechanical", hod:"Dr.Khan"}])
{
  acknowledged: true,
  insertedIds: {
    '0': ObjectId('6a869fb3a152a947acfa421a'),
    '1': ObjectId('6a869fb3a152a947acfa421b'),
    '2': ObjectId('6a869fb3a152a947acfa421c')
  }
}
collegeDB> db.students.insertOne({ name:"Vikram",age:24,dept:"CSE",marks:55})
{
  acknowledged: true,
  insertedId: ObjectId('6a86a012a152a947acfa421d')
}
collegeDB> db.students.insertMany([{name:"Anya",age:20,dept:"ECE",marks:69},{name:"Dev",age:21,dept:"MECH",marks:74}])
{
  acknowledged: true,
  insertedIds: {
    '0': ObjectId('6a86a078a152a947acfa421e'),
    '1': ObjectId('6a86a078a152a947acfa421f')
  }
}
collegeDB> db.students.insertOne({name:"Praveen",age:21,dept:"CSE",marks:90,city:"Guntur"})
{
  acknowledged: true,
  insertedId: ObjectId('6a86a106a152a947acfa4220')
}
collegeDB> db.students.find()
[
  {
    _id: ObjectId('6a869eb6a152a947acfa4214'),
    name: 'Arav',
    age: 21,
    dept: 'CSE',
    marks: 90,
    city: 'Hyderabad',
    skills: [ 'python', 'mongodb' ],
    fees: { total: 50000, paid: 30000 }
  },
  {
    _id: ObjectId('6a869eb6a152a947acfa4215'),
    name: 'Divya',
    age: 22,
    dept: 'ECE',
    marks: 72,
    skills: [ 'c', 'verilog' ],
    city: 'Chennai',
    fees: { total: 45000, paid: 45000 }
  },
  {
    _id: ObjectId('6a869eb6a152a947acfa4216'),
    name: 'Kabir',
    age: 20,
    dept: 'CSE',
    marks: 91,
    skills: [ 'java', 'sql', 'mongodb' ],
    city: 'Hyderabad',
    fees: { total: 50000, paid: 50000 }
  },
  {
    _id: ObjectId('6a869eb6a152a947acfa4217'),
    name: 'Meera',
    age: 23,
    dept: 'MECH',
    marks: 64,
    skills: [ 'autocad' ],
    city: 'Pune',
    fees: { total: 40000, paid: 20000 }
  },
  {
    _id: ObjectId('6a869eb6a152a947acfa4218'),
    name: 'Rohan',
    age: 21,
    dept: 'CSE',
    marks: 78,
    skills: [ 'python', 'sql' ],
    city: 'Chennai',
    fees: { total: 50000, paid: 40000 }
  },
  {
    _id: ObjectId('6a869eb6a152a947acfa4219'),
    name: 'Sana',
    age: 22,
    dept: 'ECE',
    marks: 88,
    skills: [ 'python', 'matlab' ],
    city: 'Hyderabad',
    fees: { total: 45000, paid: 45000 }
  },
  {
    _id: ObjectId('6a86a012a152a947acfa421d'),
    name: 'Vikram',
    age: 24,
    dept: 'CSE',
    marks: 55
  },
  {
    _id: ObjectId('6a86a078a152a947acfa421e'),
    name: 'Anya',
    age: 20,
    dept: 'ECE',
    marks: 69
  },
  {
    _id: ObjectId('6a86a078a152a947acfa421f'),
    name: 'Dev',
    age: 21,
    dept: 'MECH',
    marks: 74
  },
  {
    _id: ObjectId('6a86a106a152a947acfa4220'),
    name: 'Praveen',
    age: 21,
    dept: 'CSE',
    marks: 90,
    city: 'Guntur'
  }
]
collegeDB> db.students.findOne({ dept: "CSE"})
{
  _id: ObjectId('6a869eb6a152a947acfa4214'),
  name: 'Arav',
  age: 21,
  dept: 'CSE',
  marks: 90,
  city: 'Hyderabad',
  skills: [ 'python', 'mongodb' ],
  fees: { total: 50000, paid: 30000 }
}
collegeDB> db.students.findOne({city: "Hyderabad"})
{
  _id: ObjectId('6a869eb6a152a947acfa4214'),
  name: 'Arav',
  age: 21,
  dept: 'CSE',
  marks: 90,
  city: 'Hyderabad',
  skills: [ 'python', 'mongodb' ],
  fees: { total: 50000, paid: 30000 }
}
collegeDB> db.students.findOne({name:"Arav"})
{
  _id: ObjectId('6a869eb6a152a947acfa4214'),
  name: 'Arav',
  age: 21,
  dept: 'CSE',
  marks: 90,
  city: 'Hyderabad',
  skills: [ 'python', 'mongodb' ],
  fees: { total: 50000, paid: 30000 }
}
collegeDB> db.students.find({marks:{$gt:80}})
[
  {
    _id: ObjectId('6a869eb6a152a947acfa4214'),
    name: 'Arav',
    age: 21,
    dept: 'CSE',
    marks: 90,
    city: 'Hyderabad',
    skills: [ 'python', 'mongodb' ],
    fees: { total: 50000, paid: 30000 }
  },
  {
    _id: ObjectId('6a869eb6a152a947acfa4216'),
    name: 'Kabir',
    age: 20,
    dept: 'CSE',
    marks: 91,
    skills: [ 'java', 'sql', 'mongodb' ],
    city: 'Hyderabad',
    fees: { total: 50000, paid: 50000 }
  },
  {
    _id: ObjectId('6a869eb6a152a947acfa4219'),
    name: 'Sana',
    age: 22,
    dept: 'ECE',
    marks: 88,
    skills: [ 'python', 'matlab' ],
    city: 'Hyderabad',
    fees: { total: 45000, paid: 45000 }
  },
  {
    _id: ObjectId('6a86a106a152a947acfa4220'),
    name: 'Praveen',
    age: 21,
    dept: 'CSE',
    marks: 90,
    city: 'Guntur'
  }
]
collegeDB> db.students.find({age:{$gt:20, $lt:23}})
[
  {
    _id: ObjectId('6a869eb6a152a947acfa4214'),
    name: 'Arav',
    age: 21,
    dept: 'CSE',
    marks: 90,
    city: 'Hyderabad',
    skills: [ 'python', 'mongodb' ],
    fees: { total: 50000, paid: 30000 }
  },
  {
    _id: ObjectId('6a869eb6a152a947acfa4215'),
    name: 'Divya',
    age: 22,
    dept: 'ECE',
    marks: 72,
    skills: [ 'c', 'verilog' ],
    city: 'Chennai',
    fees: { total: 45000, paid: 45000 }
  },
  {
    _id: ObjectId('6a869eb6a152a947acfa4218'),
    name: 'Rohan',
    age: 21,
    dept: 'CSE',
    marks: 78,
    skills: [ 'python', 'sql' ],
    city: 'Chennai',
    fees: { total: 50000, paid: 40000 }
  },
  {
    _id: ObjectId('6a869eb6a152a947acfa4219'),
    name: 'Sana',
    age: 22,
    dept: 'ECE',
    marks: 88,
    skills: [ 'python', 'matlab' ],
    city: 'Hyderabad',
    fees: { total: 45000, paid: 45000 }
  },
  {
    _id: ObjectId('6a86a078a152a947acfa421f'),
    name: 'Dev',
    age: 21,
    dept: 'MECH',
    marks: 74
  },
  {
    _id: ObjectId('6a86a106a152a947acfa4220'),
    name: 'Praveen',
    age: 21,
    dept: 'CSE',
    marks: 90,
    city: 'Guntur'
  }
]
collegeDB> db.students.find({dept:"CSE", city: "Hyderabad"})
[
  {
    _id: ObjectId('6a869eb6a152a947acfa4214'),
    name: 'Arav',
    age: 21,
    dept: 'CSE',
    marks: 90,
    city: 'Hyderabad',
    skills: [ 'python', 'mongodb' ],
    fees: { total: 50000, paid: 30000 }
  },
  {
    _id: ObjectId('6a869eb6a152a947acfa4216'),
    name: 'Kabir',
    age: 20,
    dept: 'CSE',
    marks: 91,
    skills: [ 'java', 'sql', 'mongodb' ],
    city: 'Hyderabad',
    fees: { total: 50000, paid: 50000 }
  }
]
collegeDB> db.students.find({ dept:"CSE"},{name:1,marks:1,_id:0})
[
  { name: 'Arav', marks: 90 },
  { name: 'Kabir', marks: 91 },
  { name: 'Rohan', marks: 78 },
  { name: 'Vikram', marks: 55 },
  { name: 'Praveen', marks: 90 }
]
collegeDB> db.students.find({dept:{$in:["CSE","ECE"]}})
[
  {
    _id: ObjectId('6a869eb6a152a947acfa4214'),
    name: 'Arav',
    age: 21,
    dept: 'CSE',
    marks: 90,
    city: 'Hyderabad',
    skills: [ 'python', 'mongodb' ],
    fees: { total: 50000, paid: 30000 }
  },
  {
    _id: ObjectId('6a869eb6a152a947acfa4215'),
    name: 'Divya',
    age: 22,
    dept: 'ECE',
    marks: 72,
    skills: [ 'c', 'verilog' ],
    city: 'Chennai',
    fees: { total: 45000, paid: 45000 }
  },
  {
    _id: ObjectId('6a869eb6a152a947acfa4216'),
    name: 'Kabir',
    age: 20,
    dept: 'CSE',
    marks: 91,
    skills: [ 'java', 'sql', 'mongodb' ],
    city: 'Hyderabad',
    fees: { total: 50000, paid: 50000 }
  },
  {
    _id: ObjectId('6a869eb6a152a947acfa4218'),
    name: 'Rohan',
    age: 21,
    dept: 'CSE',
    marks: 78,
    skills: [ 'python', 'sql' ],
    city: 'Chennai',
    fees: { total: 50000, paid: 40000 }
  },
  {
    _id: ObjectId('6a869eb6a152a947acfa4219'),
    name: 'Sana',
    age: 22,
    dept: 'ECE',
    marks: 88,
    skills: [ 'python', 'matlab' ],
    city: 'Hyderabad',
    fees: { total: 45000, paid: 45000 }
  },
  {
    _id: ObjectId('6a86a012a152a947acfa421d'),
    name: 'Vikram',
    age: 24,
    dept: 'CSE',
    marks: 55
  },
  {
    _id: ObjectId('6a86a078a152a947acfa421e'),
    name: 'Anya',
    age: 20,
    dept: 'ECE',
    marks: 69
  },
  {
    _id: ObjectId('6a86a106a152a947acfa4220'),
    name: 'Praveen',
    age: 21,
    dept: 'CSE',
    marks: 90,
    city: 'Guntur'
  }
]
collegeDB> db.students.find({skills:"python"})
[
  {
    _id: ObjectId('6a869eb6a152a947acfa4214'),
    name: 'Arav',
    age: 21,
    dept: 'CSE',
    marks: 90,
    city: 'Hyderabad',
    skills: [ 'python', 'mongodb' ],
    fees: { total: 50000, paid: 30000 }
  },
  {
    _id: ObjectId('6a869eb6a152a947acfa4218'),
    name: 'Rohan',
    age: 21,
    dept: 'CSE',
    marks: 78,
    skills: [ 'python', 'sql' ],
    city: 'Chennai',
    fees: { total: 50000, paid: 40000 }
  },
  {
    _id: ObjectId('6a869eb6a152a947acfa4219'),
    name: 'Sana',
    age: 22,
    dept: 'ECE',
    marks: 88,
    skills: [ 'python', 'matlab' ],
    city: 'Hyderabad',
    fees: { total: 45000, paid: 45000 }
  }
]
collegeDB> db.students.find({skills:{$all:["python","sql"]})
Uncaught:
SyntaxError: Unexpected token, expected "," (1:48)

> 1 | db.students.find({skills:{$all:["python","sql"]})
    |                                                 ^
  2 |

collegeDB> db.students.find({skills:{$all:["python","sql"]}})
[
  {
    _id: ObjectId('6a869eb6a152a947acfa4218'),
    name: 'Rohan',
    age: 21,
    dept: 'CSE',
    marks: 78,
    skills: [ 'python', 'sql' ],
    city: 'Chennai',
    fees: { total: 50000, paid: 40000 }
  }
]
collegeDB> db.students.find({"fees.paid":{$lt:40000}})
[
  {
    _id: ObjectId('6a869eb6a152a947acfa4214'),
    name: 'Arav',
    age: 21,
    dept: 'CSE',
    marks: 90,
    city: 'Hyderabad',
    skills: [ 'python', 'mongodb' ],
    fees: { total: 50000, paid: 30000 }
  },
  {
    _id: ObjectId('6a869eb6a152a947acfa4217'),
    name: 'Meera',
    age: 23,
    dept: 'MECH',
    marks: 64,
    skills: [ 'autocad' ],
    city: 'Pune',
    fees: { total: 40000, paid: 20000 }
  }
]
collegeDB> db.students.find().sort({marks:-1}).limit(3)
[
  {
    _id: ObjectId('6a869eb6a152a947acfa4216'),
    name: 'Kabir',
    age: 20,
    dept: 'CSE',
    marks: 91,
    skills: [ 'java', 'sql', 'mongodb' ],
    city: 'Hyderabad',
    fees: { total: 50000, paid: 50000 }
  },
  {
    _id: ObjectId('6a86a106a152a947acfa4220'),
    name: 'Praveen',
    age: 21,
    dept: 'CSE',
    marks: 90,
    city: 'Guntur'
  },
  {
    _id: ObjectId('6a869eb6a152a947acfa4214'),
    name: 'Arav',
    age: 21,
    dept: 'CSE',
    marks: 90,
    city: 'Hyderabad',
    skills: [ 'python', 'mongodb' ],
    fees: { total: 50000, paid: 30000 }
  }
]
collegeDB> db.students.distinct("city")
[ 'Chennai', 'Guntur', 'Hyderabad', 'Pune' ]
collegeDB> db.students.updateOne({name:"Meera"},{$set:{marks:70}})
{
  acknowledged: true,
  insertedId: null,
  matchedCount: 1,
  modifiedCount: 1,
  upsertedCount: 0
}
collegeDB> db.students.updateMany({dept:"CSE"},{$inc:{marks:5}})
{
  acknowledged: true,
  insertedId: null,
  matchedCount: 5,
  modifiedCount: 5,
  upsertedCount: 0
}
collegeDB> db.students.updateMany({dept:"CSE"},{$push:{skills:"git"}})
{
  acknowledged: true,
  insertedId: null,
  matchedCount: 5,
  modifiedCount: 5,
  upsertedCount: 0
}
collegeDB> db.students.updateMany({dept:"ECE"},{$inc:{fees.total:2000}})
Uncaught:
SyntaxError: Unexpected token, expected "," (1:47)

> 1 | db.students.updateMany({dept:"ECE"},{$inc:{fees.total:2000}})
    |                                                ^
  2 |

collegeDB> db.students.updateMany({dept:"ECE"},{$inc:{fees.total:2000}})
Uncaught:
SyntaxError: Unexpected token, expected "," (1:47)

> 1 | db.students.updateMany({dept:"ECE"},{$inc:{fees.total:2000}})
    |                                                ^
  2 |

collegeDB> db.students.find()
[
  {
    _id: ObjectId('6a869eb6a152a947acfa4214'),
    name: 'Arav',
    age: 21,
    dept: 'CSE',
    marks: 95,
    city: 'Hyderabad',
    skills: [ 'python', 'mongodb', 'git' ],
    fees: { total: 50000, paid: 30000 }
  },
  {
    _id: ObjectId('6a869eb6a152a947acfa4215'),
    name: 'Divya',
    age: 22,
    dept: 'ECE',
    marks: 72,
    skills: [ 'c', 'verilog' ],
    city: 'Chennai',
    fees: { total: 45000, paid: 45000 }
  },
  {
    _id: ObjectId('6a869eb6a152a947acfa4216'),
    name: 'Kabir',
    age: 20,
    dept: 'CSE',
    marks: 96,
    skills: [ 'java', 'sql', 'mongodb', 'git' ],
    city: 'Hyderabad',
    fees: { total: 50000, paid: 50000 }
  },
  {
    _id: ObjectId('6a869eb6a152a947acfa4217'),
    name: 'Meera',
    age: 23,
    dept: 'MECH',
    marks: 70,
    skills: [ 'autocad' ],
    city: 'Pune',
    fees: { total: 40000, paid: 20000 }
  },
  {
    _id: ObjectId('6a869eb6a152a947acfa4218'),
    name: 'Rohan',
    age: 21,
    dept: 'CSE',
    marks: 83,
    skills: [ 'python', 'sql', 'git' ],
    city: 'Chennai',
    fees: { total: 50000, paid: 40000 }
  },
  {
    _id: ObjectId('6a869eb6a152a947acfa4219'),
    name: 'Sana',
    age: 22,
    dept: 'ECE',
    marks: 88,
    skills: [ 'python', 'matlab' ],
    city: 'Hyderabad',
    fees: { total: 45000, paid: 45000 }
  },
  {
    _id: ObjectId('6a86a012a152a947acfa421d'),
    name: 'Vikram',
    age: 24,
    dept: 'CSE',
    marks: 60,
    skills: [ 'git' ]
  },
  {
    _id: ObjectId('6a86a078a152a947acfa421e'),
    name: 'Anya',
    age: 20,
    dept: 'ECE',
    marks: 69
  },
  {
    _id: ObjectId('6a86a078a152a947acfa421f'),
    name: 'Dev',
    age: 21,
    dept: 'MECH',
    marks: 74
  },
  {
    _id: ObjectId('6a86a106a152a947acfa4220'),
    name: 'Praveen',
    age: 21,
    dept: 'CSE',
    marks: 95,
    city: 'Guntur',
    skills: [ 'git' ]
  }
]
collegeDB> db.students.updateMany({dept:"ECE"},{$inc:{"fees.total":2000}})
{
  acknowledged: true,
  insertedId: null,
  matchedCount: 3,
  modifiedCount: 3,
  upsertedCount: 0
}
collegeDB> db.students.find()
[
  {
    _id: ObjectId('6a869eb6a152a947acfa4214'),
    name: 'Arav',
    age: 21,
    dept: 'CSE',
    marks: 95,
    city: 'Hyderabad',
    skills: [ 'python', 'mongodb', 'git' ],
    fees: { total: 50000, paid: 30000 }
  },
  {
    _id: ObjectId('6a869eb6a152a947acfa4215'),
    name: 'Divya',
    age: 22,
    dept: 'ECE',
    marks: 72,
    skills: [ 'c', 'verilog' ],
    city: 'Chennai',
    fees: { total: 47000, paid: 45000 }
  },
  {
    _id: ObjectId('6a869eb6a152a947acfa4216'),
    name: 'Kabir',
    age: 20,
    dept: 'CSE',
    marks: 96,
    skills: [ 'java', 'sql', 'mongodb', 'git' ],
    city: 'Hyderabad',
    fees: { total: 50000, paid: 50000 }
  },
  {
    _id: ObjectId('6a869eb6a152a947acfa4217'),
    name: 'Meera',
    age: 23,
    dept: 'MECH',
    marks: 70,
    skills: [ 'autocad' ],
    city: 'Pune',
    fees: { total: 40000, paid: 20000 }
  },
  {
    _id: ObjectId('6a869eb6a152a947acfa4218'),
    name: 'Rohan',
    age: 21,
    dept: 'CSE',
    marks: 83,
    skills: [ 'python', 'sql', 'git' ],
    city: 'Chennai',
    fees: { total: 50000, paid: 40000 }
  },
  {
    _id: ObjectId('6a869eb6a152a947acfa4219'),
    name: 'Sana',
    age: 22,
    dept: 'ECE',
    marks: 88,
    skills: [ 'python', 'matlab' ],
    city: 'Hyderabad',
    fees: { total: 47000, paid: 45000 }
  },
  {
    _id: ObjectId('6a86a012a152a947acfa421d'),
    name: 'Vikram',
    age: 24,
    dept: 'CSE',
    marks: 60,
    skills: [ 'git' ]
  },
  {
    _id: ObjectId('6a86a078a152a947acfa421e'),
    name: 'Anya',
    age: 20,
    dept: 'ECE',
    marks: 69,
    fees: { total: 2000 }
  },
  {
    _id: ObjectId('6a86a078a152a947acfa421f'),
    name: 'Dev',
    age: 21,
    dept: 'MECH',
    marks: 74
  },
  {
    _id: ObjectId('6a86a106a152a947acfa4220'),
    name: 'Praveen',
    age: 21,
    dept: 'CSE',
    marks: 95,
    city: 'Guntur',
    skills: [ 'git' ]
  }
]
collegeDB> db.students.deleteMany({marks:{$lt:60}})
{ acknowledged: true, deletedCount: 0 }
collegeDB> db.students.aggregate({{$group:{_id:"$dept",avgMarks:{$avg:"$marks"}}})
Uncaught:
SyntaxError: Unexpected token (1:23)

> 1 | db.students.aggregate({{$group:{_id:"$dept",avgMarks:{$avg:"$marks"}}})
    |                        ^
  2 |

collegeDB> db.students.aggregate({{$group:{_id:"$dept",avgMarks:{$avg:"$marks"}}}})
Uncaught:
SyntaxError: Unexpected token (1:23)

> 1 | db.students.aggregate({{$group:{_id:"$dept",avgMarks:{$avg:"$marks"}}}})
    |                        ^
  2 |

collegeDB> db.students.aggregate({{$group:{_id:"$dept",avgMarks:{$avg:"$marks"}})
Uncaught:
SyntaxError: Unexpected token (1:23)

> 1 | db.students.aggregate({{$group:{_id:"$dept",avgMarks:{$avg:"$marks"}})
    |                        ^
  2 |

collegeDB> db.students.aggregate([{{$group:{_id:"$dept",avgMarks:{$avg:"$marks"},totalStudents:{$sum:1},topScore:{$max: "$marks"}}}])
Uncaught:
SyntaxError: Unexpected token (1:24)

> 1 | db.students.aggregate([{{$group:{_id:"$dept",avgMarks:{$avg:"$marks"},totalStudents:{$sum:1},topScore:{$max: "$marks"}}}])
    |                         ^
  2 |

collegeDB> db.students.aggregate([{$group:{_id:"$dept",avgMarks:{$avg:"$marks"},totalStudents:{$sum:1},topScore:{$max: "$marks"}}}])
[
  {
    _id: 'ECE',
    avgMarks: 76.33333333333333,
    totalStudents: 3,
    topScore: 88
  },
  { _id: 'CSE', avgMarks: 85.8, totalStudents: 5, topScore: 96 },
  { _id: 'MECH', avgMarks: 72, totalStudents: 2, topScore: 74 }
]
collegeDB> db.students.aggregate([{$group:{_id:"$dept",count:{$sum:1}}},{$sort:{count:-1}}])
[
  { _id: 'CSE', count: 5 },
  { _id: 'ECE', count: 3 },
  { _id: 'MECH', count: 2 }
]
collegeDB> db.students.aggregate([{$project:{name:1,pendingfees:{$sub$subtract:["$fees.total","$fees.paid"]}}},{$sort:{pendingFees:-1}}])
[
  {
    _id: ObjectId('6a869eb6a152a947acfa4214'),
    name: 'Arav',
    pendingfees: 20000
  },
  {
    _id: ObjectId('6a869eb6a152a947acfa4215'),
    name: 'Divya',
    pendingfees: 2000
  },
  {
    _id: ObjectId('6a869eb6a152a947acfa4216'),
    name: 'Kabir',
    pendingfees: 0
  },
  {
    _id: ObjectId('6a869eb6a152a947acfa4217'),
    name: 'Meera',
    pendingfees: 20000
  },
  {
    _id: ObjectId('6a869eb6a152a947acfa4218'),
    name: 'Rohan',
    pendingfees: 10000
  },
  {
    _id: ObjectId('6a869eb6a152a947acfa4219'),
    name: 'Sana',
    pendingfees: 2000
  },
  {
    _id: ObjectId('6a86a012a152a947acfa421d'),
    name: 'Vikram',
    pendingfees: null
  },
  {
    _id: ObjectId('6a86a078a152a947acfa421e'),
    name: 'Anya',
    pendingfees: null
  },
  {
    _id: ObjectId('6a86a078a152a947acfa421f'),
    name: 'Dev',
    pendingfees: null
  },
  {
    _id: ObjectId('6a86a106a152a947acfa4220'),
    name: 'Praveen',
    pendingfees: null
  }
]
collegeDB> db.students.aggregate([{$unwind:"$skills"},{$group:{_id:"$skills",count:{$sum:1}}},{$sort:{count:-1}},{$limit:3}])
[
  { _id: 'git', count: 5 },
  { _id: 'python', count: 3 },
  { _id: 'mongodb', count: 2 }
]
collegeDB> db.students.aggregate([{$lookup:{from:"departments",localField:"dept",foreignField:"dept",as:"departmentInfo"}},{$unwind:"$departmentInfo"},{$project:{_id:0,"student Name":"$name","Department":"$dept","HOD":"$departmentInfo.hod"}}])

collegeDB> db.students.aggregate([{$lookup:{from:"departments",localField:"dept",foreignField:"dept",as:"departmentInfo"}},{$unwind:"$departmentInfo"},{$project:{_id:0,"student Name":"$name","Department":"$dept","HOD":"$departmentInfo.hod"}}])

collegeDB> db.students.aggregate([{$match:{}},{$out:"Praveencollection"}])

collegeDB>
