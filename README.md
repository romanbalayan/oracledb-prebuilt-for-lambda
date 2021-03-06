# node-oracledb-prebuilt-for-lambda

 - This module is forked from the currently un-maintained [node-oracledb-for-lambda](https://github.com/nalbion/node-oracledb-for-lambda).
 - Core oracledb libraries are derived from [node-oracledb](https://github.com/oracle/node-oracledb) v5.2.0
 - 5.2.0: Prebuilt for use with AWS Lambda nodejs12.x Runtime (Built using nodejsv12.18.3)
 - Also tested to work with AWS Lambda nodejs14.x Runtime
 
The scripts to reproduce the build process can be found at [node-oracledb-lambda-test](https://github.com/romanbalayan/node-oracledb-lambda-test). 

# Usage

```bash
npm install --save oracledb-prebuilt-for-lambda@5.2.0
```

# Versioning
 - Changed release version to match that of underlying node-oracledb version. 
 - i.e. for release based on oracledb 5.2.0, release will be oracledb-prebuilt-for-lambda@5.2.0
 
 
 # Releases
 | node-oracledb       | oracledb-prebuilt-for-lambda    |
 | ------------------- | ---------- |
 | 5.2.0               | 5.2.0      |
 | 5.1.0               | 5.1.0      |
 | 5.0.0               | 5.0.0      |
 | 4.2.0               | 4.2.0      |
 | 4.1.0               | 4.1.0      |
 | 4.0.1               | 1.0.3      |

 
 # Changelog
 - v5.2.0: [node-oracledb v5.2.0 changelog](https://github.com/oracle/node-oracledb/blob/main/CHANGELOG.md#node-oracledb-v520-7-jun-2021)
 - v5.1.0: [node-oracledb v5.1.0 changelog](https://github.com/oracle/node-oracledb/blob/master/CHANGELOG.md#node-oracledb-v510-8-dec-2020)
 - v5.0.0: [node-oracledb v5.0.0 changelog](https://github.com/oracle/node-oracledb/blob/master/CHANGELOG.md#node-oracledb-v500-29-jun-2020)
 - v4.2.0: [node-oracledb v4.2.0 changelog](https://github.com/oracle/node-oracledb/blob/master/CHANGELOG.md#node-oracledb-v420-24-jan-2020)
 - v4.1.0: [node-oracledb v4.1.0 changelog](https://github.com/oracle/node-oracledb/blob/master/CHANGELOG.md#node-oracledb-v410-26-nov-2019)
 - v4.0.1: [node-oracledb v4.0.1 changelog](https://github.com/oracle/node-oracledb/blob/master/CHANGELOG.md#node-oracledb-v401-19-aug-2019)
 
 
 # AWS Lambda NodeJS Runtimes
 https://docs.aws.amazon.com/lambda/latest/dg/lambda-runtimes.html
 Data as of June 17, 2021
 
  | Name          | Identifier | Operating System  |
  | ------------- | ---------- | ----------------- |
  | Node.js 14    | nodejs14.x | AWS Linux 2       |
  | Node.js 12    | nodejs12.x | AWS Linux 2       |
  | Node.js 10    | nodejs10.x | AWS Linux 2       |
 
  
 
Due to the size of the Oracle libraries, you may need to deploy your zip file to S3 and get Lambda to download from the S3 URL.
