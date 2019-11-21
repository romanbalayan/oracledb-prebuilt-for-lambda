# node-oracledb-prebuilt-for-lambda

 - This module is derived from [node-oracledb-for-lambda](https://github.com/nalbion/node-oracledb-for-lambda). 
 - Core oracledb libraries are also derived from [node-oracledb](https://github.com/oracle/node-oracledb) v4.0.1
 - 4.0.1-10a: Prebuilt for use with AWS Lambda nodejs10.x Runtime (Built using nodejsv10.16.3)
 
The scripts to reproduce the build process can be found at [node-oracledb-lambda-test](https://github.com/romanbalayan/node-oracledb-lambda-test). 

# Usage

```bash
# nodejs10.x
npm install --save oracledb-prebuilt-for-lambda@4.0.1-10a
```

# Versioning
 - Changed release version based on release of underlying node-oracledb and lambda node runtime version. 
 - i.e. for nodejs10.x release based on oracledb 4.0.1, release will be 4.0.1-10a.
 
 
 # Releases
 | AWS Lambda Runtime  | Release    |
 | ------------------- | ---------- |
 | nodejs10.x          | 4.0.1-10a  |
 
 
 # AWS Lambda NodeJS Runtimes
 https://docs.aws.amazon.com/lambda/latest/dg/lambda-runtimes.html
 Data as of Nov 21, 2019
 
  | Name          | Identifier | Node.js Version | Operating System  |
  | ------------- | ---------- | --------------- | ----------------- |
  | Node.js 12    | nodejs12.x | 12.13.0         | AWS Linux 2       |
  | Node.js 10    | nodejs10.x | 12.13.0         | AWS Linux 2       |
  | Node.js 8.10  | nodejs8.10 | 8.10            | AWS Linux         |
  
 
Due to the size of the Oracle libraries, you may need to deploy your zip file to S3 and get Lambda to download from the S3 URL.
