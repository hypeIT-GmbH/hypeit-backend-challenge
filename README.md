# 🧠 Backend Challenge: Metal Festival API

Welcome to the backend challenge! In this task, your goal is to build a RESTful API to manage a list of metal festivals using either Java Spring Boot or Node.js with TypeScript + TypeORM.

This API will support features such as listing, filtering, creating, and retrieving detailed information about festivals.

## 🚀 Before You Start
⚠️ Important: Choose one stack:
	•	Node.js 20+ with Express, TypeScript and TypeORM (preferred)
	•	Java 17+ with Spring Boot 3.x

⚠️ Do not fork this repository.
Instead: 
1.	Create a new GitHub repository.
2.	Clone it to your local machine.
3.	Start building your solution.
4.	When you’re done, push it to your GitHub and share the link.

Alternatively, you may submit a ZIP file with your project.

## 🔧 Requirements
Your task is to create a REST API with the following Endpoints:
1. GET /festivals
    - Returns a list of all festivals.
    - Support query parameters for filtering:
        - name (partial match)
        - location (exact match)
        - from / to (date range)

2. GET /festivals/:id
    - Returns detailed information about a single festival.

3. POST /festivals
    - Creates a new festival.
    - Required fields: name, date, location
    - Optional: imageUrl, description

4. PUT /festivals/:id
    - Updates an existing festival.

### 📦 Database
You are free to choose a local database:
- MariaDB/MySQL (preferred)	
- PostgreSQL

### Festival Entity (example schema):
```json
{
  "id": "number",
  "name": "string",
  "date": "string (ISO 8601)",
  "location": "string",
  "description": "string (optional)",
  "imageUrl": "string (optional)"
}
```

## 🧪 Testing
Add at least one unit or integration test using:
- Node.js: Jest + Supertest
- Spring Boot: JUnit + MockMvc

## 🛠 Extras (Optional, But Nice)
- Input validation with proper error responses
- Pagination on list endpoint
- Caching
- Swagger or OpenAPI documentation
- Docker setup
- Seed script for demo data

## 📚 Submission
Please submit your solution by providing:
- A GitHub repo link or a ZIP file
- A README.md with setup instructions:
- How to run locally
- How to run tests
- How to access API docs (if available)

## ⏱ Scope
This task is designed to take around 4 hours. Don’t worry if you can’t complete everything — focus on clean, well-structured code and showing how you think.