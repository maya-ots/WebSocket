# QUIZ questions :
# PART 1 : 
## Q1
Which HTTP method must be used by the client for the initial WebSocket handshake request?
* A. POST
* B. GET
* C. PUT
* D. CONNECT

## Q2
What HTTP status code does a server return to indicate that it has successfully agreed to switch protocols to WebSocket?
* A. 200 OK
* B. 201 Created
* C. 101 Switching Protocols
* D. 304 Not Modified

## Q3
What HTTP status code does a server return to indicate that it has successfully agreed to switch protocols to WebSocket?
* A. 200 OK
* B. 201 Created
* C. 101 Switching Protocols
* D. 304 Not Modified

## Q1
What HTTP status code does a server return to indicate that it has successfully agreed to switch protocols to WebSocket?
* A. 200 OK
* B. 201 Created
* C. 101 Switching Protocols
* D. 304 Not Modified
## Q1
What HTTP status code does a server return to indicate that it has successfully agreed to switch protocols to WebSocket?
* A. 200 OK
* B. 201 Created
* C. 101 Switching Protocols
* D. 304 Not Modified

# PART 2
## Question 1
When a client initiates a WebSocket connection, what is the initial protocol used for the 'handshake' before the connection is upgraded?

* A) TCP

* B) WSP (WebSocket Protocol)

* C) FTP

* D) HTTP

## Question 2

In a basic Node.js chat application using 'socket.io', what is the most direct way to send a message to all connected clients, including the sender?

* A) io.emit('message', data)

* B) socket.broadcast.emit('message', data)

* C) io.sockets.emit('message', data)

* D) socket.emit('message', data)

## Question 3

What is a key advantage of using Socket.IO over the native WebSocket API ('ws' library) in Node.js for a public-facing application?

* A)
Socket.IO offers significantly faster raw data transfer speeds.

* B)
Socket.IO has built-in support for various transport mechanisms, providing fallbacks for older browsers or restrictive networks.

* C)
Socket.IO does not require a server-side component.

* D)
Socket.IO is the only library that supports binary data streaming.

## Question 4

On the client-side, when using Socket.IO, how is the connection to the server typically established in JavaScript?

* A)
By calling the 'io()' function, which is made available by the Socket.IO client-side script.

* B)
By using the 'socket.connect()' method with the server URL as an argument.

* C)
By sending a POST request to the '/socket.io/' endpoint.

* D)
By creating a new WebSocket object: 'new WebSocket('ws://localhost:3000')'.

## Question 5

What is the purpose of the 'http' module when creating a Socket.IO server, even if you are using Express?

* A)
It's only necessary for serving the client-side 'socket.io.js' file.

* B)
It's a fallback for when the 'ws' library is not installed.

* C)
It's used to create an HTTP server that the Socket.IO server can then attach to.

* D)
It's required to parse JSON data sent from the client.

## Question 6

In a Node.js chat app, if you want to send a 'user disconnected' message to all *other* clients when one client disconnects, where would you place the 'socket.broadcast.emit()' call?

* A)
Inside a 'socket.on('message', ...)' event listener.

* B)
Outside of all event listeners, at the top level of your server file.

* C)
Inside the 'socket.on('disconnect', ...)' event listener.

* D)
Inside the 'io.on('connection', ...)' callback, but before the 'socket.on('disconnect', ...)' event listener.

## Question 7

In the 'ws' library for Node.js, how do you handle incoming messages on the server?

* A)
ws.on('message', function incoming(message) { ... })

* B)
ws.listen('message', function(message) { ... })

* C)
wss.on('message', function incoming(message) { ... })

* D)
wss.receive(function(message) { ... })

## Question 8

What is a potential issue with a simple chat app where the server immediately broadcasts every received message using 'io.emit()'?

* A)
This will not work if there are more than two clients connected.

* B)
It's not possible to send private messages between users.

* C)
It can cause a memory leak on the server.

* D)
The sender will not receive their own message.

## Question 9

How does Socket.IO's 'disconnection detection' feature enhance the reliability of a real-time application?

* A)
It sends a daily report of all disconnections to the server administrator.

* B)
It automatically switches to a different server if the current one becomes unavailable.

* C)
It allows both the client and server to be aware of when the connection is lost, enabling cleanup or UI updates.

* D)
It prevents clients from ever disconnecting from the server.

## Question 10

When serving the client-side Socket.IO script, why is it typically included with '<script src='/socket.io/socket.io.js'></script>'?

* A)
The Socket.IO server automatically creates this endpoint to serve the client-side library.

* B)
You must manually create a route in your Express app to serve this file

* C)
This script is only for debugging and should be removed in production

* D)
This is a public CDN URL that hosts the script for everyone