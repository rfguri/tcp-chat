# tcp-chat

This is a *super* basic TCP server that anyone can connect to without implementing any sophisticated protocols or commands:

  * When the server is connected, it greets you and asks for you name. It tells you how many other clients are connected.
  * Upon typing in your name followed by Enter, you're considered connected.
  * When connected, you can receive and send messages to other connected clients by typing and pressing Enter.


## Usage instructions

Run this code to spawn your TCP to the server:

    $ node server.js

When ***listen*** executes, it binds the server to the port ***3000*** and subsenquetly prints a message to the server terminal. An important method is ***listen***, which allows you to *bind the server to a port*. Because this method is *asynchronous*, it also receives a *callback*.

Whithin several terminals run this code to attemp a connection with ***telnet***:

    $ telnet 127.0.0.1 3000

If that connection goes as expected, you will see the command and the *"new connection!"* output side by side.

To kill one terminal you could run:

    $ ps aux | grep telnet
    $ kill -9 <telnet-pid>

## Usage Image

![tcp-chat image](https://raw.githubusercontent.com/rogerfernandezg/tcp-chat/master/tcp-chat.png "tcp-chat image")

## Licence

The MIT License (MIT)

Copyright (c) 2013 Roger Fernandez Guri

Permission is hereby granted, free of charge, to any person obtaining a copy of
this software and associated documentation files (the "Software"), to deal in
the Software without restriction, including without limitation the rights to
use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
the Software, and to permit persons to whom the Software is furnished to do so,
subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
