#### Request and Reponse Client Side

#### Table of Contents
- [Intro](#intro)
- [HTTP Requests](#http-requests)
- [AJAX Requests](#ajax-requests)
- [Response](#response)


# Intro
The way a client (e.g a browser) accesses data on the web (e.g. a webpage) is by sending a request to a server.
The client does this to either access data or change data on the server.

# HTTP Requests
The most common protocol for these requests is HTTP which usually consists of:
- Method
	- This is the action the client wants the server to do. This is often one of:
		- Get
			- This is retrieving data from the server, e.g a web page.
			- An idempotent operation.
			- A safe method as it doesn't change the server's state.
		- Post
			- Sends data to update or create a resource, e.g submitting a form.
			- Non-idempotent (i.e. creating multiple new users can result in different outcomes).
		- Put
			- Updates or replaces an existing resource on the server.
			- Idempotent as even though we're changing the server 
				- Changing the same thing in the same way results in the same outcome.
		- Delete
			- Deletes a specified resource on the server.
			- Idempotent for similar reasons as put.
- URL
        - This is the resource that the client wants to access.
- Headers
	- Additional information, not included in the body.
	- E.g. browser type, authentication tokens.
- Body
        - Option, contains data needed for the action.
	- Often used for Post or Put commands.

# AJAX Requests
- This uses JavaScript code to allow the client to send requests which don't require reloading the entire page.
- This is used to allow for dynamic elements on web-pages which the user can interact with. 

# Response 
- The response from the server that the client receives typically includes:
	- Status code
		- Indicates the result of the request.
		- E.g: 
			- 200 means success.
			- 300 means the data requested has been moved .
			- 400 means an error.
	- Headers
		- Information about the response.
		- For example, the content type of the body.
	- Body
		- The actual content.
		- For example the html of a web page.












































































































































































