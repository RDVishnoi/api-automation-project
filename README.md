📄 README.md
# 🧪 User Management API Automation

This project demonstrates automated REST API testing using Postman and Newman, integrated with CI/CD.

---

## 📌 Project Overview

This mini automation framework validates user-related APIs using:

- Postman Collection
- Newman CLI
- JavaScript assertions
- GitHub Actions (CI/CD ready)

The project simulates real-world API automation practices followed in industry.

---

## 🛠 Tech Stack

- Postman
- Newman
- Node.js
- JavaScript
- Git & GitHub

---

## 🌐 API Used

Public test API:
https://dummyjson.com

Endpoints Covered:

- GET /users
- GET /users/{id}
- POST /users/add

---

## 📂 Project Structure



api-automation/
│
├── User_API.postman_collection.json
├── qa.postman_environment.json
├── package.json
├── .gitignore
└── README.md


---

## ✅ Test Scenarios Automated

- Validate response status code (200)
- Validate response body structure
- Validate user ID correctness
- Validate user creation response

---

## ▶️ How To Run Locally

### 1️⃣ Install Dependencies



npm install


### 2️⃣ Run Tests



npm test


OR



npx newman run User_API.postman_collection.json
-e qa.postman_environment.json


---

## ⚙️ CI/CD Integration

This project supports GitHub Actions.

On every push to `main` branch:

- Node.js is installed
- Newman is installed
- API tests are executed automatically
- Build fails if any test fails

---

## 📊 Sample Output



✓ Status code is 200
✓ Users list exists
✓ Correct user returned


If any assertion fails, the pipeline turns red ❌.

---

## 🚀 Future Improvements

- HTML test reporting
- Schema validation
- Data-driven testing
- Retry logic for flaky network
- Slack/email notifications

---

## 👨‍💻 Author

Your Name
Ram
