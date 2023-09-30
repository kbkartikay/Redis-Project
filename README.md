
# Redis

Remote Dictionary Server(Redis) which is a fast, in-memory, key-value data store implemented in C++.

The Redis server handles GET, SET and DEL commands concurrently using Event Loop and Socket Programming.

For key value store a Chaining Hash Table is used as an Intrusive Data Structure



## Deployment

To deploy this project first compile all the files :
```bash
g++ -o server 09_server.cpp
g++ -o client 09_client.cpp
g++ -o hashtable hashtable.cpp
```
Open a new terminal and start the server using cmd : 
```bash
./server 
```
In another terminal we can run a client instance with get, set and del commands passed as command line arguments
```bash
./client set k v
./client get k
./client del k
```

