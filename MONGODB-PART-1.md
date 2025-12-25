# Mongodb

***************************************************PART-1***************************************************************************************

1.start with mongosh(In cmd)


2.Ctrl + L(This is the shortcut to clear the mongoshell)

3.for database checking use
show dbs


4.for using database
use college

5.for colllections
show collections


6.MongoDB stores data in Documents (BSON) inside Collections.
"Basic structure"
{
  name: "al",
  age: 18,
  status: "D",
  groups: ["politics", "news"]
}

7.for inserting data
//insert one
db.student.insertOne({ name: "kamlakant", age: 22, marks: 88 })


//insert many
db.student.insertMany([
  { name: "jitendra", age: 24, course: "btech" },
  { name: "priyanshu", age: 25, course: "diploma" }
])


8.FOR FINDING THE DATA USE
==>db.student.find()
==>db.student.find({ city: "gujarat" })
==>db.student.findOne({ name: "kamlakant" })

9.FOR QUERY OPERATORS USE
==>db.student.find({ marks: { $gt: 75 } })
==>db.student.find({ marks: { $gte: 80 } })
==>db.student.find({ city: { $in: ["gujarat"] } })


10.FOR UPDATION OF DATA
==> UPDATING ONE DOCUMENT
db.student.updateOne(
  { name: "kamlakant" },
  { $set: { marks: 99 } }
)
==>UPDATING MANY DOCUMENT
db.student.updateMany(
  { city: "gujarat" },
  { $set: { city: "ahmedabad" } }
)


11.FOR UPDATE OPERATORS
==>OPERATOR
$set
$addFields
$project
$unset
$replaceRoot
$replaceWith

12.FOR NESTING STRUCTURE
==>INSERT NESTED DOCUMENT
db.student.insertOne({
  name: "farah",
  performance: {
    marks: 88,
    grade: "A"
  }
})
==>FIND NESTED FIELD
db.student.findOne({ "performance.marks": 88 })


13.DIFFRERENCE BETWEEN JSON AND BSON
==>
JSON	                                   BSON
UTF-8 String	                           Binary Format
Limited Datatypes	                       Extra datatypes like Date, Long, Decimal128
Human Readable	                         Machine Optimized

14.SCREENSHOTS OF ALL THE RESOURCES ARE GIVEN BELOW
![WhatsApp Image 2025-12-22 at 11 37 19 AM](https://github.com/user-attachments/assets/8f57092b-0211-4747-a551-4a27306e6f14)
![WhatsApp Image 2025-12-23 at 6 15 54 PM](https://github.com/user-attachments/assets/65895f58-96dc-4b63-a257-133489f8093d)
![WhatsApp Image 2025-12-23 at 6 22 10 PM](https://github.com/user-attachments/assets/acbb72db-55d8-4f53-a226-490887a94856)
![WhatsApp Image 2025-12-23 at 6 23 00 PM](https://github.com/user-attachments/assets/94bd42f6-dec7-4242-a18c-7b2791c7cc71)
<img width="570" height="173" alt="image" src="https://github.com/user-attachments/assets/55373e82-007f-4df1-b7dc-63c03606e590" />

![WhatsApp Image 2025-12-23 at 6 38 16 PM](https://github.com/user-attachments/assets/9d2e2ec8-8f85-4c73-99d5-def4183a3094)

<img width="1089" height="471" alt="image" src="https://github.com/user-attachments/assets/7bab45b9-6004-4dd5-96c5-87f795ba0075" />

<img width="1124" height="766" alt="image" src="https://github.com/user-attachments/assets/f23e6f00-3d97-44a4-833f-6e7f339c719a" />

<img width="1237" height="755" alt="image" src="https://github.com/user-attachments/assets/90880132-5fa5-427f-92bc-3c1416d9c21a" />


<img width="1487" height="277" alt="image" src="https://github.com/user-attachments/assets/4b6316f1-b287-4325-bd69-7e0334915581" />


<img width="1081" height="905" alt="image" src="https://github.com/user-attachments/assets/3a527ae5-f308-4611-a218-b83b7cbf41a3" />


<img width="1409" height="578" alt="image" src="https://github.com/user-attachments/assets/4b0d3432-db28-4944-ba49-39ccc065d1fa" />

<img width="1600" height="329" alt="image" src="https://github.com/user-attachments/assets/0e9a64ce-2ced-4d5c-a1d5-1af64e935c32" />


<img width="1512" height="865" alt="image" src="https://github.com/user-attachments/assets/049bd588-c456-461d-97ad-46ed8e91800e" />

<img width="1028" height="660" alt="image" src="https://github.com/user-attachments/assets/9d7d941b-5a67-4206-87f3-1757a2fd2a58" />


<img width="822" height="963" alt="image" src="https://github.com/user-attachments/assets/780deb49-2d9d-45ec-b57a-cad3bb8543a2" />

<img width="1331" height="907" alt="image" src="https://github.com/user-attachments/assets/8e6205a0-62ea-454e-b953-dd0e6d526051" />

<img width="716" height="996" alt="image" src="https://github.com/user-attachments/assets/91eb69d7-bdf7-4b08-a0e6-cc218f525a35" />

<img width="1444" height="679" alt="image" src="https://github.com/user-attachments/assets/208e03fa-9db0-4185-b05d-bf15c51508c7" />

<img width="565" height="731" alt="image" src="https://github.com/user-attachments/assets/f9cbedb0-7478-4032-8637-7d4c36ed3726" />

<img width="834" height="955" alt="image" src="https://github.com/user-attachments/assets/11b1270b-8a8e-4414-9bd3-560020b3f76b" />

<img width="1143" height="879" alt="image" src="https://github.com/user-attachments/assets/4cf66bfc-02e6-4b76-b24c-7565c2e05f35" />

<img width="914" height="758" alt="image" src="https://github.com/user-attachments/assets/a8f357a3-4deb-4d92-ac3d-a8db4338216c" />

<img width="968" height="375" alt="image" src="https://github.com/user-attachments/assets/7a2c093b-617f-4fb9-ae35-d71df5bc5242" />
































