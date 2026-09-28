# simpleAPI
This demo makes the app server a bit more realistic. It emulates a database by providing data in an array for the frontend to request

The application is written using named functions to improve readability until you get used to this stuff

The endpoints are:


GET  http://localhost:3000 to simply output a message

GET  http://localhost:3000/results to return all results in the array

POST http://localhost:3000/results to add a new student to the array (database). Data is posted in JSON or url-encoding format

GET  http://localhost:3000/results/name?lName={name} to get the results of the named student

GET  http://localhost:3000/results:id to get the results for student with the provided id

PATCH http://localhost:3000/results:id/newName updates only a specific field in a record. Find the record by id then update the last name

## Calling the endpoints
As we can only GET using the browser we need a different tool to test this. Postman is popular. I quite like the liteClient vscode extension as you can write the endpoints in a file and call from there. 

Note the file containing the endpoints to test is ***.rest***

This tool enables us to test the backend without needing an html / css / JavaScript frontend