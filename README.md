# Chat client and server

Coded a simple chat client. You can set IP:PORT and nickname at runtime using command-line arguments. This code reads non-blocking without echo.


The chat-server is compatible with the chat-client. This code can handle multiple users simultaneous. 

Chat Protocol
Client	Direction	Server
Connect()	-->	
<--	Hello <VERSION>
NICK <nick>	-->	
<--	OK/ERR <text>
MSG <text>	-->	
<--	MSG nick <text>/ERROR <text>
Nicknames is limited to 12 characters (A-Za-z0-9\_) and messages is limited to 255 characters (any characters except control characters and newlines, utf-8 encoding).
Each message is followed by newline (CR).

 


