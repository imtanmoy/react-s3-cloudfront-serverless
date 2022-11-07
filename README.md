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
5. Replace the `bucketName` in `serverless.yml` with your own bucket name. Remember that bucket names must be globally unique.
6. Set environment variables in `serverless.yml` for `ACM_CERTIFICATE_ARN`, `ROUTE53_RECORD_SET_NAME`, and `ROUTE53_HOSTED_ZONE_ID`
7. Run `serverless deploy --stage dev --verbose`
