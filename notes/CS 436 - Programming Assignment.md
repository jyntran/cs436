# CS 436 - Programming Assignment

- 1 control connection
	- ServerSocket on server side
- 1 data connection
	- ServerSocket on client side

- this is to be similar to FTP

## Client

1. connect to server
2. sends command 
3. receives "OK"
4. create ServerSocket for data connection on available port #
	- Hint: Google
5. send port # to server
	- Hint: Java ServeSocket class
	- send client address
	- Hint: send the host name (java inetaddress class)
6. sends message over data connection
7. close data connection
8. as long as command is not EXIT, loops

## Server

1. establishes
2. wait for connection with client
3. receives command
4. sends OK
5. wait for port #, address (host name)
6. create connection for data connection
7. receive message
8. send transformed message