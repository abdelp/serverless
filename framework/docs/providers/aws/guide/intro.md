# Serverlss Framework Concepts

## Functions

**Where is the code of a serverless application deployed?**

The code of a serverless application is deployed and executed in AWS Lambda functions.

**Where is a function?**

Each function is an independent unit of execution and deployment, like a microservice.
A function is merely code, deployed in the cloud, that is most often written to perform a single job.

## Events

## Resources

**What are resources?**

Resources are AWS infraestructure components which your functions use such as:

* A DynamoDB table
* An S3 bucket
* An SNS topic
* Anything that can be defined in CloudFormation is supported by the Serverless Framework

## Services

**What's a service?**

A service is the Framework's unit of organization. You can think of it as a project file, though you can have multiple services for a single application.

**How is a service configured?**

A service is configured via a `serverless.yml` file where you define your functions, events and AWS resources to deploy.

**What happens when you deploy with the Framework via the serverless deploy?**

When deploying with the Framework via `serverless deploy`, everything in the configuration file is deployed at once.

## Alternative configuration format

**How can you define the service configuration in case of needing more flexibility?**

In case you need more flexibility, you can also define the service configuration in:

* JSON (`serverless.json`)
* JavaScript (`serverlese.js`)
* Typescript (`serverless.ts`)

## Plugins

**How can you overwrite or extend the functionality of the Framework?**

You can overwrite or extend the functionality of the Framework using plugins. Every `serverless.yml` can contain a `plugins:` property, which features multiple plugins.

