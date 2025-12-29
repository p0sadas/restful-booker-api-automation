# Automated API Testing Suite - Restful Booker 🚀

This project demonstrates a comprehensive automated testing strategy for the **Restful Booker API**, utilizing **Postman** and **JavaScript**.

## 🎯 Project Objectives
* Validate full **CRUD** lifecycles (Create, Read, Update, Delete).
* Implement security and authentication tests using **Bearer Tokens**.
* Demonstrate advanced **Environment Variable** management and **Request Chaining**.
* Execute **Negative Testing** and **Edge Cases** to ensure API resilience.

## 🛠️ Tech Stack
* **Postman** (Web App)
* **JavaScript** (Validation and automation scripts)
* **JSON Schema** (Data structure and contract validation)

## 📂 Collection Structure
1. **Auth:** Dynamic generation of access tokens.
2. **Happy Path:** Successful flow for creating, fetching, and editing bookings.
3. **Negative Testing:** Validation of 401 (Unauthorized), 403 (Forbidden), and 404 (Not Found) error codes.
4. **Edge Cases:** Testing for date logic, character limits, and basic script injection.

## 🚀 How to Run the Project
1. **Clone** this repository.
2. **Import** the file `collections/restful-booker-collection.json` into Postman.
3. **Import** the file `environments/restful-booker-env.json`.
4. Ensure the **Environment** is selected in the top-right corner.
5. Click the **Run** button on the collection to execute all tests automatically.

## 📈 Key Findings (QA Insights)
* **Contract Testing:** Implemented **JSON Schema** validations to ensure every response complies with the API's data contract.
* **Automation:** Automated the extraction of `bookingid`, eliminating the need for manual data entry between requests.
* **Logic Vulnerabilities:** Documented date handling inconsistencies (Edge Cases) where the API allows a checkout date prior to the checkin date.
