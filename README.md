# node-oracledb-prebuilt-for-lambda

This module is a derived from [node-oracledb-for-lambda](https://github.com/nalbion/node-oracledb-for-lambda). Updated to support NodeJS10.x AWS Lambda Runtim
This module is a fork of [node-oracledb](https://github.com/oracle/node-oracledb) v4.0.1

The scripts to reproduce the build process can be found at [node-oracledb-lambda-test](https://github.com/nalbion/node-oracledb-lambda-test). 

# Usage

In addition to the usual package.json and *.js files, you also need to include the 
Oracle Instant Client libraries provided in `lambda-lib` - they should be in your zip file's `lib/` directory.

```bash
npm install --save oracledb-prebuilt-for-lambda

zip app.zip index.js package.json \
   your-other-dependencies... \
   node_modules/oracledb-prebuilt-for-lambda/package.json \
   node_modules/oracledb-prebuilt-for-lambda/index.js \
   node_modules/oracledb-prebuilt-for-lambda/lib/*.js \
   node_modules/oracledb-for-lambda/build/Release/oracledb.node \
   lib/*.so* \
```

Due to the size of the Oracle libraries, you may need to deploy your zip file to S3 and get Lambda to download from the S3 URL.
