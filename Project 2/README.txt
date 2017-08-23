Make sure ftserver.c and ftclient.py are in different directories!
Also, when running the program, the client and the server need to be on different versions of flip (flip2, flip3).
This program was tested with flip2 and flip3.

To compile ftserver.c, just type make. Then, type ./ftserver [port number] to start the server (where port number is the number you want to run the server on).
To start the client, give it executable permissions with chmod +x ftclient.py.
To use the client to get a specific file, type python ftclient.py [server name (flip2 for example)] [server port (where you started the server)] -g [file name] [data port]
For example, I had test.txt in the server directory so I typed python ftclient.py flip3 30158 -g test.txt 30159

To use the client to get the directory list, type python ftclient.py [server name] [server port] -l [data port]
Another example: python ftclient.py flip3 30158 -l 30159.