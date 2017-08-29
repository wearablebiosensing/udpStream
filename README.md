# udpStream
Python Socket Streaming

This code is to be deployed for basic data streaming via Sockets

Codes included
Server - the host with data to stream - udpdatastream.py
Controller - the controlling client initiating a data stream - udpcontroller.py
StreamR - a client to receive the data stream - udpstreamreceiver.py

Server is the primary controller and must be up and running before any clients (controller and data StreamR) can connect
ie:
>> python udpdatastream.py

Once Server is running, connect the clients
ie:
>> python udpcontroller.py localhost 9009
>> python udpstreamreceiver.py localhost 9009

To initiate data streaming, send anything at all from the controller
ie:
>> [Controller] go

Data will begin streaming. To exit the stream press ^C

This program serves as an example and must be modified for use in an application
