📚 Book Management REST API (Node.js + Express)

A simple and beginner-friendly REST API built using Node.js and Express.js to manage a list of books.
This project demonstrates the core concepts of CRUD operations, Express routing, middleware, JSON handling, and API testing using Postman.

🚀 Features

✔ GET – Fetch all books
✔ POST – Add a new book
✔ PUT – Update a book by ID
✔ DELETE – Delete a book by ID
✔ Uses in-memory storage (no database)
✔ Clean and minimal Express server setup
✔ Fully testable in Postman

🛠 Tech Stack

Node.js

Express.js

Postman (for API testing)

📦 Installation & Setup
1️⃣ Clone or Download the Project
git clone <your-repo-link>

2️⃣ Install Dependencies
npm install

3️⃣ Start the Server
node server.js

4️⃣ Server Runs On:
http://localhost:3000

🗂 Project Structure
book-api/
│── server.js       # Main Express server
│── package.json    # Project metadata & dependencies
│── README.md       # Documentation

🧠 API Endpoints
📘 1. Get All Books

GET /books
Returns the list of all books.

✔ Response Example
[
  {
    "id": 1,
    "title": "Book One",
    "author": "Author A"
  }
]

➕ 2. Add a New Book

POST /books
Send JSON body:

{
  "title": "My New Book",
  "author": "Ayesha"
}

✔ Response
{
  "id": 3,
  "title": "My New Book",
  "author": "Ayesha"
}

✏ 3. Update a Book

PUT /books/:id
Example URL:

http://localhost:3000/books/1

✔ Request Body
{
  "title": "Updated Book",
  "author": "Updated Author"
}

✔ Response
{
  "id": 1,
  "title": "Updated Book",
  "author": "Updated Author"
}

❌ 4. Delete a Book

DELETE /books/:id

Example URL:

http://localhost:3000/books/1

✔ Response
{
  "message": "Book deleted successfully"
}

🔍 Testing Instructions (Postman)

Open Postman Desktop App

Choose the correct HTTP method (GET/POST/PUT/DELETE)

Enter URL:

http://localhost:3000/books


For POST and PUT → go to Body → raw → JSON

Add JSON data and click Send

View responses in the Postman output window




