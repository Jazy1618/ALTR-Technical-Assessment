## ALTR's DATA & Platform Technical Challenge - HTTP  

Please complete the user stories below:

---

Scenario: HTTP Webserver Implementation       
When: An HTTP request is received  
Then: The webserver determines if the requesting client has exceeded the request limit of 3 requests per IP address per 30 seconds. If the limit has been exceeded, the webserver is expected to reject the request. If the limit is not exceeded, the webserver is expected to successfully service the request.  


---

Scenario: HTTP Client library Implementation    
When: A Node.js application calls the HTTP client library  
Then: The HTTP client library issues a request to the aforementioned HTTP webserver. If the HTTP request is rejected, the request is expected to be retried with exponential back off. If the request is serviced successfully, the results are expected to be returned to the invoking function.  

---

Scenario: Unit tests  
When: The command `npm test` is executed in the parent directory  
Then: Unit test(s) will successfully pass with code coverage that exceeds 95%. Tests are expected to be written for both the HTTP client library as well as the HTTP webserver.