# Playwright TypeScript API Automation Framework

A robust API Automation Framework built using **Playwright** and **TypeScript** following industry best practices. This project automates REST API testing for complete **CRUD (Create, Read, Update, Delete)** operations with request validation, response verification, and HTML reporting.

---

# Project Overview

This framework demonstrates REST API automation using Playwright. It covers the complete lifecycle of API testing by validating CRUD operations and ensuring reliable API behavior through comprehensive assertions.

The framework includes:

* Create (POST)
* Read (GET)
* Update (PUT/PATCH)
* Delete (DELETE)
* Status Code Validation
* Response Body Validation
* Header Validation
* Authentication Support
* HTML Reports

---

# Tech Stack

| Technology | Version |
| ---------- | ------- |
| Playwright | Latest  |
| TypeScript | Latest  |
| Node.js    | 18+     |
| npm        | Latest  |

---

# Project Structure

```text
Playwright-API-Automation
│
├── tests/
│   ├── CreateUser.spec.ts
│   ├── GetUser.spec.ts
│   ├── UpdateUser.spec.ts
│   └── DeleteUser.spec.ts
│
├── playwright.config.ts
├── package.json
├── package-lock.json
├── tsconfig.json
└── README.md
```

---

# Framework Features

* Playwright API Testing
* TypeScript
* CRUD Operations
* REST API Validation
* Authentication Support
* Response Validation
* Header Validation
* HTML Reporting
* CI/CD Ready
* Easy to Maintain and Extend

---

# API Operations Covered

## Create Resource (POST)

**Validates:**

* Status Code
* Response Body
* Generated Resource ID
* Response Time

**Endpoint Example**

```http
POST /users
```

---

## Read Resource (GET)

**Validates:**

* Status Code
* Response Body
* Resource Details
* Response Headers

**Endpoint Example**

```http
GET /users/{id}
```

---

## Update Resource (PUT)

**Validates:**

* Updated Data
* Status Code
* Response Body
* Data Persistence

**Endpoint Example**

```http
PUT /users/{id}
```

---

## Delete Resource (DELETE)

**Validates:**

* Successful Deletion
* Status Code
* Resource Removal

**Endpoint Example**

```http
DELETE /users/{id}
```

---

# Prerequisites

Before running the project, ensure the following are installed:

* Node.js (v18 or later)
* npm
* Git
* Visual Studio Code (Recommended)

---

# Installation

Clone the repository

```bash
git clone <repository-url>
```

Navigate to the project directory

```bash
cd Playwright-API-Automation
```

Install dependencies

```bash
npm install
```
#### Install Playwright & Select Configurations
- npm init playwright@latest
- 
Install Playwright browsers

```bash
npx playwright install
```

---

# Running Tests

Run all tests

```bash
npx playwright test
```

Run a specific test

```bash
npx playwright test tests/CreateUser.spec.ts
```

Run tests in headed mode

```bash
npx playwright test --headed
```

Run tests in debug mode

```bash
npx playwright test --debug
```

Run tests with a single worker

```bash
npx playwright test --workers=1
```

---

# Test Reports

After execution, open the Playwright HTML Report:

```bash
npx playwright show-report
```

---

# Assertions Covered

The framework validates:

* HTTP Status Codes
* Response Body
* Response Headers
* Response Time
* JSON Properties
* API Success Responses

Example:

```typescript
expect(response.status()).toBe(201);

const responseBody = await response.json();

expect(responseBody.name).toBe("John");

expect(response.ok()).toBeTruthy();
```

---

# Sample CRUD Execution Flow

```text
Create Resource
      │
      ▼
Retrieve Resource
      │
      ▼
Update Resource
      │
      ▼
Retrieve Updated Resource
      │
      ▼
Delete Resource
      │
      ▼
Verify Resource Deletion
```

---

# Reports

The framework generates:

* HTML Report
* Console Execution Logs
* Test Summary

---

# Best Practices Implemented

* Playwright Test Runner
* TypeScript
* Independent Test Cases
* Clear Assertions
* Readable Test Structure
* Scalable Framework Design
* REST API Best Practices

---

# Useful Commands

Install dependencies

```bash
npm install
```

Install Playwright

```bash
npx playwright install
```

Execute all tests

```bash
npx playwright test
```

Execute a single test

```bash
npx playwright test tests/CreateUser.spec.ts
```

Debug tests

```bash
npx playwright test --debug
```

Open HTML report

```bash
npx playwright show-report
```

---

# Author

**Akhila Gandikota**

**Senior QA Automation Engineer**


