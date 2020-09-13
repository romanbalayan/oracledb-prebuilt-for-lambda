# node-oracledb-prebuilt-for-lambda

 - This module is forked from the currently un-maintained [node-oracledb-for-lambda](https://github.com/nalbion/node-oracledb-for-lambda). 
 - Core oracledb libraries are also derived from [node-oracledb](https://github.com/oracle/node-oracledb) v4.1.0
 - 4.1.0: Prebuilt for use with AWS Lambda nodejs12.x Runtime (Built using nodejsv12.18.3)
 
The scripts to reproduce the build process can be found at [node-oracledb-lambda-test](https://github.com/romanbalayan/node-oracledb-lambda-test). 

# Usage

```bash
npm install --save oracledb-prebuilt-for-lambda@4.1.0
```

# Versioning
 - Changed release version to match that of underlying node-oracledb version. 
 - i.e. for release based on oracledb 4.1.0, release will be oracledb-prebuilt-for-lambda@4.1.0
 
 
 # Releases
 | node-oracledb       | Release    |
 | ------------------- | ---------- |
 | 4.0.1               | 1.0.3      |
 | 4.1.0               | 4.1.0      |
 
 
 # AWS Lambda NodeJS Runtimes
 https://docs.aws.amazon.com/lambda/latest/dg/lambda-runtimes.html
 Data as of Nov 21, 2019
 
  | Name          | Identifier | Operating System  |
  | ------------- | ---------- | ----------------- |
  | Node.js 12    | nodejs12.x | AWS Linux 2       |
  | Node.js 10    | nodejs10.x | AWS Linux 2       |
 
  
 
Due to the size of the Oracle libraries, you may need to deploy your zip file to S3 and get Lambda to download from the S3 URL.
