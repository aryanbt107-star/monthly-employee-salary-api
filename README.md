# Monthly Employee Salary API

A REST API built using Node.js, Express.js, and MySQL for retrieving monthly employee salary information from the HRMS database.

## Features

* Fetch monthly salary details for a specific employee
* View basic salary and final salary
* View present days and total monthly working days
* Employee-wise and month-wise salary lookup
* MySQL database integration

## Tech Stack

* Node.js
* Express.js
* MySQL
* REST API
* Postman
* Git & GitHub

## API Endpoint

### Get Monthly Employee Salary

```http
GET /salary/monthly/:employeeId/:month
```

### Example Request

```http
GET /salary/monthly/21/2024-11
```

### Sample Response

```json
{
  "employeeId": 21,
  "employeeName": "Avduth Kemble",
  "month": "2024-11",
  "basicSalary": "9500",
  "finalSalary": "5502.00",
  "presentDays": "13",
  "monthlyDays": 30
}
```

## Project Structure

```text
monthly-employee-salary-api
│
├── routes
│   └── salary.js
│
├── db.js
├── server.js
├── package.json
└── README.md
```

## How to Run

1. Clone the repository
2. Install dependencies

```bash
npm install
```

3. Configure MySQL database credentials in `db.js`

4. Start the server

```bash
node server.js
```

5. Test the API

```http
http://localhost:3000/salary/monthly/21/2024-11
```

## Author

Aryan Thakur
# monthly-employee-salary-api
REST API built with Node.js, Express.js, and MySQL to retrieve monthly employee salary records, including basic salary, final salary, present days, and monthly working days.
