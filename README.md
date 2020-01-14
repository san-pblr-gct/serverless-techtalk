# serverless-demo

To install serverless <br />
npm install serverless -g

npm install serverless-secrets-plugin --save-D (for serverless secrets)

npm install serverless-domain-manager --save-dev (for Custom domain)

To configure Aws node js template <br />
serverless create -t aws-nodejs

To configure AWS credentials and save in profile <br />
serverless config credentials --provider aws --key XXXXX --secret XXXXX --profile EFDEV

The environment variables are hidden in secrets.dev.yml and it is explicitly ignored while checkin using gitignore. Only the encrypted file is checked in. Encryption is done using the below command

serverless encrypt --stage dev --password 'test'

To decrypt it:
serverless decrypt --stage dev --password 'test'




