1. POST /CMS/create-site
	- return configurations that will be figured in the php file and mobile app.
	- json structure
  ```
		{
		  "agentId": "string",
		  "prefix": "string",
		  "siteId": 0,
		  "status": true,
		  "message": "",
		  "errorCode": "200"
		}
  ```

2. POST /Sites/register
    - [x] add 2 params: 'prefix' and 'agentId'. Both of them were figured in the php file.

3. POST /KV/login
    - [x] add 2 params: 'prefix' and 'agentId'. Both of them were figured in app.
  
4. POST /Sites/login
    - [x] add 2 params: 'prefix' and 'agentId'. Both of them were figured in app.
  
5. POST /KV/register
    - [x] add 2 params: 'prefix' and 'agentId'. Both of them were figured in app.
    - [x] change name of parameter 'refCode' => 'referalCode'

6. GET /Sites/get-otp/
    - [x] add 2 params: 'prefix' and 'agentId'. Both of them were figured in app.
    
7. GET /Sites/reset-password/
    - [x] add 1 params: 'otp' was gotten from /Sites/get-otp/
    
8. GET /CMS/admin/get-list
    - [x] get list of admin
