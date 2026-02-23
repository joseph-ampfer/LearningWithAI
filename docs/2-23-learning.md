Used AI to learn about client/server authority, and remote procedure calls.

RPCs are a way to basically call a function to run on someone elses device. As a client, you can call a [ServerRPC] to make a request to the server, and the server will run that function and check your request (to prevent cheating). As the server, you can call a [ClientRPC] which will run that function on all the clients. It is a way for the host to respond to clients if they need to (tell them to run animations... etc.).

