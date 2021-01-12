# Fault Tolerant File Sharing System



In this project I implemented a file sharing technique between two or more clients and server using sockets with FTP features.  The client and server uses the socket programming to connect and communicate with each other. The main feature of our application Fault tolerance is achieved by keeping  two servers, a main server and a backup server. Both servers have their own repositories having the updated files. .. Both servers will be in sync and active all the time. If the main server goes down the client will connect to the back server details.  An intermediate server takes care of providing the client with the appropriate IP address and port number of the active server. The servers are using the multithreading to provide concurrency so that it can provide services to a large number of clients at once. Finally, all the communication, in and out from client and servers, are all encrypted to provide security from sniffing of data. The client connects to the intermediate server to get the active servers IP address and port number. The client makes a TCP connection with the server, the server authenticates the client using data (username and password) stored in the form of text file. Client connects with the server to perform various features such as download, upload and listing files. No two users can access the same file together from the server due to mutex lock. In addition, a  security feature is added by encrypting the files being transferred using DES algorithm 

DEFINED SERVICES:
The following services incorporated in Project:

>> List all  files in the server,
>> Upload an Image or file to the server,
>> Download an Image or file from the server,
>> User Authentication,
>> Concurrent services to clients,
>> Secured file sharing,
>> Fault Tolerance
>> Prevent overwriting of files
>> Synchronization between servers
