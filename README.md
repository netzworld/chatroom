# Chatroom idea based from [this reddit comment](https://www.reddit.com/r/cpp/comments/1mdosph/comment/n6605hu/)
 Write a simple terminal based chatroom app (1990's style IRC).

-    Must be written in C++
-    Only external library that can be used is Boost's ASIO (networking). STL and standard c++ are all that you should use

- Only needs to run on a Linux system

- There should be two programs, a server and a client

Server acts as a simple chatroom, which when a client sends a message, the server sends it out to all the other clients.

Use multi threading to handle accepting data over the network and then sending it out to all other clients

Clients can connect to a chatroom with a desired name (passed in as a command line argument)

-    If a user types in /exit they then should gracefully disconnect

-    On standard input, when the user types a message and presses <enter> that message is sent to the server

-    Any other messages they received from the server can be printed at this time

Don't worry about any fancy stuff right now, just get these core features done

