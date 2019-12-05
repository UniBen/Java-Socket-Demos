Java Socket Demos

Dr Gary Allen, The University of Huddersfield

[![Try in PWD](https://raw.githubusercontent.com/play-with-docker/stacks/master/assets/images/button.png)](https://labs.play-with-docker.com/?stack=https://raw.githubusercontent.com/UniBen/Java-Socket-Demos/master/docker-compose.yml)

Two Java Socket Demos for use by students.

Server1 is a single threaded server that can only handle a single client and shuts down when the client terminates the connection.  It echoes strings received from client back to the client and shuts down on receipt of string "bye".  Connect to it with nc, ssh, etc.

Server4 is a multi-threaded server that can handle any number of simultaneous client connections.  It starts a separate process thread to handle each client.  Each thread terminates when the client sends a string "bye".  The server itself must be shut down by external means (i.e. killing the process), otherwise it will run indefinitely.  Connect to it with nc, ssh, etc. or with the bespoke Client4.

Client4 is a GUI client to connect to Server4.

These may all be updated over time, and other demos may be added.


