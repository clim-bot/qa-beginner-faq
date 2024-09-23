## API Testing
API Testing is the process of verifying that an API (Application Programming Interface) works as expected by sending requests to various endpoints and checking the responses. API tests focus on:

- Functionality: Does the API do what it's supposed to?
- Performance: How fast is the API?
- Security: Is the API secure from unauthorized access?

### Key Tools for API Testing:
- Postman
- REST Assured
- SoapUI

### Example:
Let's say we have an API endpoint that returns user data when you send a GET request to /users/{id}.

1. Test Case: Get User Details
- Method: GET
- Endpoint: /users/1
- Expected Result: The response should return the user's details (name, email, etc.).
- Sample Request:
```http
GET /users/1 HTTP/1.1
Host: api.example.com
```
- Expected Response:
```json
{
  "id": 1,
  "name": "John Doe",
  "email": "john@example.com"
}
```

API testing ensures that all the endpoints of an API work as expected, handle errors properly, and meet performance standards.

## CRUD
CRUD stands for Create, Read, Update, Delete, which are the four basic operations performed on a database or data resource through an API or application.

### CRUD Operations:
- Create: Adds new data.
```sql
INSERT INTO users (name, email) VALUES ('John Doe', 'john@example.com');
```
- Read: Retrieves data.
```sql
SELECT * FROM users WHERE id = 1;
```
- Update: Modifies existing data.
```sql
UPDATE users SET email = 'john.new@example.com' WHERE id = 1;
```
- Delete: Removes data.
```sql
DELETE FROM users WHERE id = 1;
```

CRUD is fundamental for managing data in databases or APIs.

### Additional Notes
- HTTP (HyperText Transfer Protocol): A protocol used for transferring data between a web browser and a server. It’s not encrypted, meaning the data can be intercepted.
```
Example: http://example.com
```
- HTTPS (HyperText Transfer Protocol Secure): A secure version of HTTP that encrypts data using SSL/TLS, protecting it from interception. It’s commonly used for secure transactions.
```
Example: https://example.com
```
- URL (Uniform Resource Locator): The web address used to locate a resource on the internet, like a webpage, image, or video. It consists of the protocol (e.g., HTTP/HTTPS), domain, and path.
```
Example: https://www.example.com/page
```

In short, HTTP transfers data, HTTPS transfers it securely, and URLs are the addresses to access resources on the web.

### HTTPS Methods
- GET: Retrieve data from the server (read-only).
- POST: Submit data to the server (creates new resources).
- PUT: Update an existing resource completely.
- PATCH: Partially update an existing resource.
- DELETE: Remove a resource from the server.
- OPTIONS: Request information about what HTTP methods are allowed on a specific resource.
- HEAD: Same as GET, but only retrieves the headers, not the full content.

### HTTP Status Code
#### 1xx: Informational
- 100 Continue: The request can continue.
- 101 Switching Protocols: Switching to a different protocol.
#### 2xx: Success
- 200 OK: The request succeeded.
- 201 Created: A new resource was created.
- 204 No Content: Request succeeded, but no content to return.
#### 3xx: Redirection
- 301 Moved Permanently: The resource has been moved to a new URL.
- 302 Found: Temporary redirect to a different URL.
#### 4xx: Client Errors
- 400 Bad Request: The request was invalid.
- 401 Unauthorized: Authentication is required.
- 403 Forbidden: Access is denied.
- 404 Not Found: The resource could not be found.
#### 5xx: Server Errors
- 500 Internal Server Error: A generic server error occurred.
- 502 Bad Gateway: The server received an invalid response from an upstream server.
- 503 Service Unavailable: The server is currently unavailable.
These codes indicate the outcome of an HTTP request.
