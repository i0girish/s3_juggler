# s3_juggler
a first hand try at AWS Lambdas

## README begins

first i created an IAM user which i linked to my vs code console.
IAM username: vscodeuser  IAM password:Vscode123#
after finishing up the set-up which was moe or less speed through i entered us-east virgenia as area in vs code.

-> npm install -g serverless

-> next I initiated a serverless file by ```serverless create --template aws-nodejs --path .```

-> ```npm init``` to get the package.json

-> ```npm install papaparse```, this will create package-lock.json

-> the serverless.yml file is responsible for lambda side actions
-> json contains any executable function.
-> this tutorial is csv to json project and has code for that in nodejs (https://www.youtube.com/watch?v=BRRxQbSb9bo)
-> did some debugging coz code didnt go as expected

->next we should setup user profile which can be done as ```code ~/.aws/credentials```

->the code is run with ```serverless invoke local stage dev --aws-profile vscodeuser -f firstlambda```

->to deploy as lambda function: ```serverless deploy --stage dev --aws-profile default ```

->to check logs we run it again but not locally this time ```serverless invoke --stage dev --aws-profile default -f firstlambda ```

=============== END dated 4 October 2022=================

## (5 Oct 2022)

utilizing previous gained knowledge to make a lambda function directly in aws console along with triggers and events which backs up data from one s3 to other bucket.

->first created a policy which was further used in role making .

->this role was used in making lambda function which didnt really go well as the tutorial didmt help in triggers
->looking for a new version!.
