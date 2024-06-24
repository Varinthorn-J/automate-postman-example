
- **testcases/**: Contains Postman collection JSON files for different test scenarios.
- **environments/**: Holds Postman environment JSON files corresponding to different environments (e.g., QA, PPE).
- **result/**: Directory to store test results, including HTML reports.
- https://www.npmjs.com/package/newman-reporter-htmlextra 

## Automated Testing with Newman

### Prerequisites
- Node.js installed
- npm installed

### Running Tests Locally
To run tests locally using Newman, follow these steps:

1. Install Newman globally:
2. Install htmlextra
- npm install -g newman-reporter-htmlextra
3. newman --version
4. Execute tests for QA environment:
5. Execute tests for PPE environment:
      
#1
   newman run testcases/products-api/producrs-api.postman_collection.json -e environments/qa/products-api/product-api.postman_environment.json -r htmlextra --reporter-htmlextra-export ./results/report.html 
#2
newman run shopping-cart-success -d data/test-data.json -e environment/local.json -r htmlextra --reporter-htmlextra-export ./results/report.html
#3
newman run testcases/customer-profile-api/Test_Script_Postman.postman_collection.json -r htmlextra --reporter-htmlextra-export ./results/report.html# automate-postman-example
# automate-postman-example
