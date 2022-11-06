# react-s3-cloudfront-serverless

Deploying a React app to S3 and CloudFront is a common task for many developers. This project shows how to do it using Serverless.

## Prerequisites

- [Node.js](https://nodejs.org/en/)
- Serverless CLI
- AWS Account

## Setup

1. Clone the repo
2. Run `yarn install`
3. Run `serverless config credentials --provider aws --key YOUR_KEY --secret YOUR_SECRET`
4. Run `yarn build`
5. Run `serverless deploy --stage dev --verbose`
