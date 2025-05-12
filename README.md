# 3b.CREATION FOR CHAT USING TCP SOCKETS
NAME:vutukuri sai kumar Reddy

REG NO:212224230307
## AIM
To write a python program for creating Chat using TCP Sockets Links.
## ALGORITHM:
1. Import the necessary modules in python
2. Create a socket connection to using the socket module.
3. Send message to the client and receive the message from the client using the Socket module in
 server
4. Send and receive the message using the send function in socket.
## PROGRAM
## client:
```
import socket
s=socket.socket()
s.connect(('localhost',8000))
while True:
    msg=input("Client>")
    s.send(msg.encode())
    print("Server>",s.recv(1024).decode())
```
## server:
```
import socket
s=socket.socket()
s.bind(('localhost',8000))
s.listen(5)
c.addr=s.accept()
while True:
    ClientMessage=c.recv(1024).decode()
    print("Client>",ClientMessage)
    msg=input("Server>")
    c.send(msg.encode())
```
    

## OUPUT
## client:
![image](https://github.com/user-attachments/assets/0177e27e-1203-4d8c-bb18-8a4c8c45dc52)
## server:
![image](https://github.com/user-attachments/assets/7137023f-ecc0-4509-9bb4-c1037f8eb335)


## RESULT
Thus, the python program for creating Chat using TCP Sockets Links was successfully 
created and executed.
