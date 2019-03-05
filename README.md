# OverTheWire_Bandit_Tutorial
Tutorial for levels 0-26 of OverTheWire's The Bandit Game, with usage of Windows OS and PuTTY SSh client.

My aim is to explain every single term with details through the whole tutorial, which should create a decent basic knowledge about Linux OS and it's utilities. 

# Level 0
 The goal of first level is to connect the Bandit's game server via SSH. Now, the first question is, what is SSH? 
 
 <h3>SSH</h3>
 <p>
 SSH, in other words, Secure Shell protocol, is a way to securely connect the Shell of a computer, or server, as we're going to mention it with this name. What is this Shell? Shell is a program, that makes the connection between user input, and the OS itself. In Linux systems, this process is usually controlled by "Bash", a short for "Bourne Again Shell". Then what is this "Terminal"? Terminal is another program, that lets you interfere with Shell, and provides you a nice terminal-like GUI. 
  </p>
 
Too many terms, and too complicated? Okay, I will try to put it all simply:

[Our PC]  ----SSH---> [Server] / We create a connection between our computer and the server with SSH <br>
[Terminal] ----Shell----> [OS] / We send commands to Shell program, which is usually Bash, and it sends the commands to OS for us. With SSH, we don't interfere with Terminal, but while we're managing the server we can use it to access Shell. 

Now if everything is clear, we need to make this SSH connection! But how? First, we need an SSH client. A program to help us make this connection. I will be using PuTTY for Windows OS. You may use another client, or you can download it from the link below: <br>
https://www.putty.org/

![PuTTY Client with Bandit Settings](https://imgur.com/peCbPz3.png)

Now let's look at the informations we're given:
The server address we need to connect is: bandit.labs.overthewire.org
The port which will accept our SSH request is: 2220
Username and Password is: bandit0

Now first, I set the address and port number, and click "Open" on PuTTY. This opens up a shell connection to the server, which asks for username and password. After entering "bandit0" in both, I gain the access. 

[PuTTY Shell](https://i.imgur.com/sdjIMkY.png)

Finally, we set the connection, we can roam in the server freely! Now our goal is, to find the password which will give us access to Level 1, and it's somewhere in this server. To see what do we have in hand, I use the "ls" command, ls is a short for List, and it lists the files in the directory I'm in.
```
bandit0@bandit:~$ ls
readme
```
This is my output. There's a file named readme. Well, let's read it then? To read it, I need to use another utility: Cat! Yes, the cat. It's the short for "concatenate" and does many useful things. This time, we will use it to read what's inside this file:
```
bandit0@bandit:~$ cat readme
boJ9jbbUNNfktd78OOpsqOltutMc3MY1
```
Voila! Here's our password for the next level.

# Level 1

Will be added soon...


