# jsonplaceholder-demo

## Automated API tests

**Requirements:**
- node.js v10.15.3
- newman

**To run and see results in console:**
newman run Jsonplaceholder_demo.postman_collection.json -e jsonplaceholder.postman_environment.json -r cli,emojitrain

**To run and save results into html file:**
newman run Jsonplaceholder_demo.postman_collection.json -e jsonplaceholder.postman_environment.json -r html --reporter-html-export reports/$(date +%d_%m_%Y)/report_$(date +%H-%M-%S-%m_%d_%Y).html
