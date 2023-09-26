# [GET] 
([https://github.com/Laura-Novich-OBW/student-showcase/tree/main/student-work/2022/Debbie-Mankowitz/api-final-project])

## What is HTTP?
The Hypertext Transfer Protocol (HTTP) is designed to enable communications between clients and servers.
HTTP works as a request-response protocol between a client and server.
Example: A client (browser) sends an HTTP request to the server; then the server returns a response to the client. The response contains status information about the request and may also contain the requested content.
## HTTP Methods
•	GET
## The GET Method
GET is used to request data from a specified resource.
Note that the query string (name/value pairs) is sent in the URL of a GET request:

## GET/TableNo
Method	syntax

## GET	URL/{tableNo}
Description
Gets the bill for a specific table number.

## Query Parameters
Name	Description
ID	The table number. The default is 99, the value for take-out orders. For POC stage, this is the only available value.

## Request
curl -X GET "http://URL/tableNo?id=99"

Response
{
   "orderNum":456,
   "timestamp":"2023-01-14T16:45:48-2:00",
   "Item1":{
  	"ItemOrdered":{
     	"type":"burgerMeal",
     	"Cost":15.99
  	}
   },
   
  	}
   }
}
