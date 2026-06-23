# E-Commerce API Test Suite 

## Overview
Industry-level automated API testing framework 
for E-Commerce application built with Postman and Newman.

## Author
Vishal Chandrabanshi
QA Engineer

## Tech Stack
- Postman (API Testing)
- Newman (CLI Runner)
- Jenkins (CI/CD Pipeline)
- GitHub (Version Control)

## Modules Tested
- Authentication (Login)
- Products (GET, POST, PUT, DELETE, Search)
- Users (GET, POST, DELETE)

## Test Coverage
- 52 automated test cases
- Status code validation
- Response time validation
- Response body validation
- Dynamic data with Pre-request scripts
- Environment based testing (QA/Dev)
- Token based authentication

## How to Run Locally
npm install -g newman
npm install -g newman-reporter-htmlextra

newman run collections/EcommerceAPI.postman_collection.json 
-e environments/QA_Environment.postman_environment.json 
-r htmlextra

## CI/CD
Tests run automatically via Jenkins pipeline
Results available as HTML report
