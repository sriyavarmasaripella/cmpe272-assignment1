# CMPE 272 - Microservices Architecture Assignment

This project demonstrates a simple microservices architecture using **Python** and **Flask**.  
It contains two independent services:

1. **User Service** (manages users, runs on port 5001)  
2. **Order Service** (manages orders, runs on port 5002, and fetches user details from User Service)

---

## 🛠 Setup Instructions

### 1. Create Virtual Environment
```bash
python3 -m venv myenv
source myenv/bin/activate      # Mac/Linux

