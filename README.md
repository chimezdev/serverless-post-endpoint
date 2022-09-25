# continued from the 'serverless-on-aws' repository

# CREATING A POST REST API ENDPOINT
We want to create a post method that we can use to add new item to our dynamodb database.

# Steps
- An item needs an id. We will use the uuid dependency to automatically generate an id for our item.
- The name and description values for the item will be provided by the client.
- Fork this repository and run `npm install` to intall the uuid and 'aws-sdk' dependencies.
- run the command `zip -r dynamodb-create.zip .` to package the codes into a zip file required by aws lambda.
- create a new lambda function say `create-group`
- click on the dropdown 'upload from' and select zip file
- upload the zip file created
- click on the configuration tab and select environment variables and add the 'GROUPS_TABLE' and <name of the dynamodb table>
- click on the permissions tab and select the execution role assigned to the lambda function.
- edit the permission to allow our function to write to the database.


