# Serverless-nodejs-primer
This is a basic setup (aka scaffolding) to help create, run and deploy a serverless app using Lambda w/ Node.js

## Technologies in use:
Below are a list of technologies that I used to develop and deploy this serverless application

* Serverless Framework - develop, deploy, and troubleshoot serverless applications. [More info](https://www.serverless.com/framework/docs/)

* Serverless-offline - is a serverless framework plugin that is pretty good at emulating AWS Lambda and the API gateway on a local machine. [More info](https://www.npmjs.com/package/serverless-offline)

* AWS

* AWS Lambda


## Install / Create Project

Install serverless 
```
$ npm install -g serverless
```

Create a new project/service - [ref link](https://www.serverless.com/framework/docs/providers/aws/cli-reference/create/)
```
$ serverless create --template aws-nodejs --name my-special-service
```

## Run app locally

You will need to install serverless-offline to allow you to run it locally

```
$ npm install serverless-offine
```

update serverless.yml with a plugin section, similar to:
```
plugins:
    - serverless-offline
```