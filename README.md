# Student Records API (AWS Lambda + DynamoDB)

This project is a serverless web application using **AWS Lambda**, **Amazon DynamoDB**, and **API Gateway**.  
It provides CRUD operations for student records.

---

## API Endpoints

`BASE_URL = https://<your-api-id>.execute-api.<region>.amazonaws.com/dev`

- **POST /students** → Create a student  
- **GET /students?student_id=123** → Get a student  
- **PUT /students** → Update a student  
- **DELETE /students?student_id=123** → Delete a student  

---

## How to Run
1. Create DynamoDB table `StudentRecords` (Partition key = student_id).  
2. Deploy Lambda function (`student_handler.py`).  
3. Connect API Gateway methods (POST, GET, PUT, DELETE).  
4. Deploy API and test using Postman/cURL.  

---

## Screenshots
(See the `screenshots/` folder for proof of working API calls.)  

- DynamoDB table view  
- POST response  
- GET response  
- PUT response  
- DELETE response  

---

## Reflection
- **Challenges:** e.g., IAM permissions, CORS errors, debugging Lambda  
- **Solutions:** e.g., checked CloudWatch logs, enabled CORS, added correct IAM policy  
- **Learnings:** Using serverless (Lambda + DynamoDB), testing APIs with Postman  

