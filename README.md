# 2b IMPLEMENTATION OF SLIDING WINDOW PROTOCOL
## AIM
IMPLEMENTATION OF SLIDING WINDOW PROTOCOL
## ALGORITHM:
1. Start the program.
2. Get the frame size from the user
3. To create the frame based on the user request.
4. To send frames to server from the client side.
5. If your frames reach the server it will send ACK signal to client
6. Stop the Program
## PROGRAM
## Client.PY
~~~Python
import socket
s=socket . socket()
s. bind(( ' localhost' , 800))
s. listen (5)
size=int(input("Enter number of frames to send
1=1 ist(range(size))
s=int(input("Enter Window Size
st=e
while True:
while(i<len(l)):
st+=s
c. send(str(l[i:st]).encode())
ack=c . recv(1Ø24) . decode()
if ack:
print(ack)
i+=s
~~~

## Server.PY
~~~Python
import socket
s=socket . socket()
s. connect(( 'localhost' , 800) )
while True:
print (s . recv(1e24) . decode())
s. send("acknowledgement recived from the server" .encode())
~~~

## OUPUT
![image](https://github.com/user-attachments/assets/58263716-f945-4de2-b549-7475c3060a32)

## RESULT
Thus, python program to perform stop and wait protocol was successfully executed
