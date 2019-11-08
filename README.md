# node-oracledb-prebuilt-for-lambda

 - This module is derived from [node-oracledb-for-lambda](https://github.com/nalbion/node-oracledb-for-lambda). 
 - Core oracledb libraries are also derived from [node-oracledb](https://github.com/oracle/node-oracledb) v4.0.1
 - Prebuilt for use with AWS Lambda nodejs10.x Runtime (Built using nodejsv10.16.3)
 
The scripts to reproduce the build process can be found at [node-oracledb-lambda-test](https://github.com/romanbalayan/node-oracledb-lambda-test). 

# Usage

```bash
npm install --save oracledb-prebuilt-for-lambda
```

Due to the size of the Oracle libraries, you may need to deploy your zip file to S3 and get Lambda to download from the S3 URL.
