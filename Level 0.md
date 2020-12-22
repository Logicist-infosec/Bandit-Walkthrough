# Level 0


>### Level Goal
The goal of this level is for you to log into the game using SSH. The host to which you need to connect is bandit.labs.overthewire.org, on port 2220. The username is bandit0 and the password is bandit0. Once logged in, go to the Level 1 page to find out how to beat Level 1.
>
>### Commands you may need to solve this level
>`ssh`
>
>### Help Reading Material
>[SSH on Wikipedia](https://en.wikipedia.org/wiki/SSH_(Secure_Shell))  
>[How to use SSH on wikiHow](https://www.wikihow.com/Use-SSH)

### Answer
Run command `ssh bandit0@bandit.labs.overthewire.org -p 2220`, then enter the password when being asked for.

### Notes
Use option `-p` to designate the port to connect, the default port number for ssh service is 22.
