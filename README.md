# Serverless Offline Sync Service

This is a serverless backend that is designed to allow syncing the DynamoDB data with the offline end client users.

## Setup

Set the required environment variables in <code>config/.env.dev</code> and <code>config/.env.pro</code> depending on the environment you want to deploy to.

```s
# create the AWS IAM user for the deployment
aws configure --profile serverless-offline-sync-service-user
# install serverless cli globally if you haven't done so
npm install -g serverless
# install dependencies
yarn install
# deploy to dev environment
sls deploy --stage dev --profile serverless-offline-sync-service-user
# deploy to production environment
sls deploy --stage pro --profile serverless-offline-sync-service-user
```