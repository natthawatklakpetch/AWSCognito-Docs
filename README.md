# AWSCognito-Docs.

Concept of Pool

User Pool

  handle user registration, authentication, and account recovery.

  Example:
    1.You created a new application.
    2.But you don't have the following system in your app yet:
        Register system.
        Log in/Log out system.
        User Interface for register system.
        Authentication system.
    3.You use AWS Cognito "User Pool" Service.
        By using only SDK you can solve the above problem. 
      
Identity Pool

   If you want the user to secure access your other AWS Service(Ex. S3,DynamoDB). 
   You need to authorize your users to Identity Pool first.
   
   and the user that will authorize with Identity Pool to access the AWS Service. Doesn't need to came from only User Pool
   but also from the other source
   https://d33wubrfki0l68.cloudfront.net/4602d3b127c9b3f1dbe49f9fc77e8d8a4aff20a6/9c3a1/assets/cognito-user-pool-vs-identity-pool.png
   
   Example:
      1.You want your user to Upload files to S3 Bucket.
      2.You will use the Identity Pool.
          While creating your Identity Pool in AWS console you can set how much access the use user has.

So in summary; the Cognito User Pool stores all your users which then plugs into your Cognito Identity Pool which can give your users access to your AWS services.

Function available for UserPool and 

https://docs.aws.amazon.com/cognito/latest/developerguide/using-amazon-cognito-user-identity-pools-javascript-examples.html
https://serverless-stack.com/chapters/cognito-user-pool-vs-identity-pool.html
