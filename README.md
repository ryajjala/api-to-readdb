# api-to-readdb
sample-code to learn aws apigateway


Lambda function that is triggered by api gateway to read and display random word from a collection of words in dynamodb

## **Steps for creating this demo**
API Gateway API route: 

CustomAPI : readDB is created

Lambda Function: with the script is deployed. 

DynamoDB table with items : word:car , word:truck, word:banana created

Testing from Client: 

install client using npm : npm install wscat

using WSCAT: 

wscat --connect < api websocket endpoint> 
#after connection is established send message from client to trigger lambda

{"action":"readDB","message":"read"}
