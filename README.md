# 🧠 Backend Challenge: Metal Festival API

Welcome to the backend challenge! Your goal is to build a RESTful API to manage a list of metal festivals using either Java Spring Boot or Node.js with TypeScript and TypeORM.

This API should support features such as listing, filtering, creating, and retrieving detailed information about festivals. Develop it as if it were going to production the next day, and you wouldn’t be able to debug it.

## 🚀 Before You Start
⚠️ Important: Choose one stack:
- Node.js 20+ with Express, TypeScript, and TypeORM (preferred)
- Java 17+ with Spring Boot 3.x

⚠️ Do not fork this repository.
Instead: 
1.	Create a new GitHub repository.
2.	Clone it to your local machine.
3.	Start building your solution.
4.	When you’re done, push it to your GitHub and share the link.

Alternatively, you may submit a ZIP file containing your project.

## 🔧 Requirements
Your task is to create a REST API with the following endpoints (use meaningful endpoint names):
1. Load festivals
    - Returns a list of all festivals.
    - Supports query parameters for filtering:
        - `name` (partial match)
        - `location` (exact match)
        - `from` / `to` (date range)

2. Load one festival
    - Returns detailed information about a single festival.

3. Create festival
    - Creates a new festival.
    - Required fields: `name`, `date`, `location`
    - Optional fields: `imageUrl`, `description`

4. Update festival
    - Updates an existing festival.

5. Delete festival
    - Deletes an existing festival.

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
- Pagination for the list endpoint
- Caching
- Swagger or OpenAPI documentation
- Docker setup
- Seed script for demo data

## 📚 Submission
Please submit your solution by providing:
- A GitHub repository link or a ZIP file
- A `README.md` with setup instructions:
  - How to run the project locally
  - How to run tests
  - How to access API documentation (if available)

## ⏱ Scope
This task is designed to take around 4 hours. Don’t worry if you can’t complete everything — focus on writing clean, well-structured code and demonstrating your thought process.