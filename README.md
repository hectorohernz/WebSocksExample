# Web Socket Example

Steps to write a WebSocket echo server based on the net/http library, you need to:

1. Initiate a handshake 
2. Receive data frames from the client 
3. Send data frames to the client
4. Close the handshake






The first thing we’ll have to do is to define a websocker.Upgrader struct. This will hold information such as the Read and Write buffer size for our WebSocket connection:
var upgrader = websocket.Upgrader{
   ReadBufferSize:  1024,
  WriteBufferSize: 1024,
}