# Expense Sharing API

> A RESTful Java API that helps groups track and split shared expenses fairly. 
Ideal for roommates, friends traveling together, or teams managing shared costs.

## 🛠️ Features
- Create users and groups
- Add shared expenses with split logic
- View who owes whom
- Settle balances
- Track group expenses over time


## 🚀 Getting Started

### Tech Stack

- Java 21.0.6
- Spring Boot
- REST API (Spring MVC)
- MySQL (configured via `application.yml`)
- JPA / Hibernate
- Gradle

### Prerequisites
- Java 11+
- Maven / Gradle
- Any IDE like IntelliJ or Eclipse

### Installation

Clone the repo:
```bash
git clone https://github.com/pinkish-code/expense-sharing-API.git
```
### Run the App
```bash
mvn spring-boot:run
```
The API will start on: http://localhost:8080

### Project Structure
src/
├── main/
│   ├── java/
│   │   └── org.example
│   │       ├── controller/
│   │       ├── service/
│   │       ├── model/
│   │       └── repository/
│   └── resources/
│       └── application.yml
└── test/

### Sample API Endpoints
**|Method   | **Endpoint**  |         Description   |**
POST	    /users	            Create a new user
POST	    /groups	            Create a group
POST	    /expenses	        Add an expense to a group
GET	        /balances/{groupId}	Get balance sheet for a group
POST	    /settle	            Record a settlement transaction


### Example: Add Expense Payload json 

{
"groupId": 1,
"payerId": 2,
"amount": 120.0,
"description": "Dinner at Joe's",
"splitBetween": [1, 2, 3]
}
### Contributions
Contributions welcome! Please open an issue or submit a pull request.











