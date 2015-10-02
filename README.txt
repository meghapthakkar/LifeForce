This project provides a clustered architecture of server systems.
Upon server startup, a leader is chosen using flood max algorithm. This leader becomes a load balancer.
The server topology is mesh.
The client is built in python. 
Google's Protocol buffers are used to send messages between client and server and also amongst the servers.
Load balancer strategy:
Real time load on each computer, and current number of requests on each node. By combining these two factors, we determined node with most available resources and chose that server to handle incoming request.
