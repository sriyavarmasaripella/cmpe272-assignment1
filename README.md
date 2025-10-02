# Microservices Assignment - CMPE 272

This project demonstrates a simple microservices architecture using **Python** and **Flask**.

---

## Services

### 1. User Service (`user_service.py`)
- Runs on port **5001**
- Create and retrieve users
- Example:
  - Get User: `http://localhost:5001/users/1`

### 2. Order Service (`order_service.py`)
- Runs on port **5002**
- Create and retrieve orders
- Fetches user details from User Service
- Example:
  - Get Order: `http://localhost:5002/orders/1`

---

## Setup Instructions

```bash
# Create virtual environment
python -m venv myenv

# Activate environment
# On macOS/Linux:
source myenv/bin/activate
# On Windows:
myenv\Scripts\activate

# Install dependencies
pip install flask requests

# Run services
python user_service.py
python order_service.py
