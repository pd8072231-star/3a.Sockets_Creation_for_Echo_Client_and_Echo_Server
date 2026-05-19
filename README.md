# 3a.CREATION FOR ECHO CLIENT AND ECHO SERVER USING TCP SOCKETS
# AIM
To write a python program for creating Echo Client and Echo Server using TCP
Sockets Links.
## ALGORITHM:
1. Import the necessary modules in python
2. Create a socket connection to using the socket module.
3. Send message to the client and receive the message from the client using the Socket module in
 server .
4. Send and receive the message using the send function in socket.
## PROGRAM
DEVELOPED BY P.DHARSHINI

REGISTER NUMBER:212225040071
```CLIENT
import socket 
s=socket.socket() 
s.bind(('localhost',7000)) 
s.listen(5) 
c,addr=s.accept() 
while True: 
    ClientMessage=c.recv(1024).decode() 
    c.send(ClientMessage.encode())
SERVER
import socket 
s=socket.socket() 
s.connect(('localhost',7000)) 
while True: 
    msg=input("Client > ") 
    s.send(msg.encode()) 
    print("Server > ",s.recv(1024).decode())
```

## OUPUT
CLIENT
<img width="1917" height="1079" alt="image" src="https://github.com/user-attachments/assets/bc38d57e-ec8c-4214-8b21-ca8c2ff082a4" />
SERVER
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/47d7cdcc-11e2-4156-9843-6271d024a57f" />

## RESULT
Thus, the python program for creating Echo Client and Echo Server using TCP Sockets Links 
was successfully created and executed.
