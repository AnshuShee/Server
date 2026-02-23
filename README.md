Student CGPA API (In-Memory JSON Database)


Live Links

Render Deployment:


https://server-jd5g.onrender.com/students

Postman Documentation:


https://documenter.getpostman.com/view/50862709/2sBXcGCeNv

Objective

Build a REST API using Express.js that manages student CGPA records stored in an in-memory JSON array.

The application:

Uses only GET routes

Includes static and dynamic routes

Follows REST principles

Returns proper HTTP status codes

Does not use any database

Tech Stack

Node.js

Express.js

CORS

In-memory JSON data

Student Data Structure
{
  "id": 1,
  "name": "Aarav Sharma",
  "branch": "CSE",
  "semester": 8,
  "cgpa": 9.3
}
Implemented Routes
1. GET /students

Returns all students.
Status: 200

2. GET /students/topper

Returns the student with highest CGPA.
Status: 200 / 404

3. GET /students/average

Returns average CGPA.

Response:

{
  "averageCGPA": 8.12
}
4. GET /students/count

Returns total number of students.

Response:

{
  "totalStudents": 10
}
5. GET /students/:id

Returns student by ID.
Status: 200 / 404

6. GET /students/branch/:branchName

Returns students by branch.


Status: 200 / 404 or empty array

Run Locally

Clone the repository

git clone https://github.com/your-username/student-cgpa-api.git

Install dependencies

npm install

Start the server

npm start

Open in browser

http://localhost:3000/students
Author

Anshu Shee
