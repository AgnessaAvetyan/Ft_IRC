# Ft_IRC
ft_irc is a C++98 Internet Chat server for Linux.
The server needs to work with real IRC clients. For this server the irssi and kiwiirc clients were used. Multiple servers can be linked to each other to create an IRC network.

# Connect
If you'd like to try our server without having to build it you can connect to our public server shibrc.ml using the password password with the following commands :

- First install a client, here we'll use **irssi** since it is the one we chose to do the project with :
```sudo apt install irssi``` or install with **brew** if you are at 42 : ```brew install irssi```<br />
Then simply connect to the server using this command : ```irssi -c shibrc.ml -w password```

## :computer: USAGE

Run **make**, then ```./ircserv <port> <password>```

## Handled commands
This following list of commands are handled on our server.

- INVITE
- JOIN
- KICK
- LIST
- NAMES
- PART
- TOPIC
- NICK
- QUIT
- PING
- PONG
- NOTICE
- PRIVMSG
- WHO
- WHOIS
- WHOWAS

## Handled modes :
The following list of modes are handled by the server, yet again there may be omitted functionnality or errors :

### USER MODES :
- a : away
- i : invisible
- w : wallops
- r : restricted
- o : operator

### CHANNEL MODES :
for users :
- O : channel creator
- o : channel operator
    
for channels :
- i : invite only
- m : moderated

## Resources

2-minute Intro to IRC: https://www.youtube.com/watch?v=-4ab5-F72nY

IRC server implementation in Node.js: https://github.com/song940/node-irc

RFC for IRC: https://datatracker.ietf.org/doc/html/rfc1459#section-1.1

Guide for ft_irc (in Russian): https://www.youtube.com/watch?v=I9o-oTdsMgI

Creating a TCP Server in C++: https://www.youtube.com/watch?v=cNdlrbZSkyQ

~~epoll(7) — Linux manual page: https://man7.org/linux/man-pages/man7/epoll.7.html~~ (doesn't work on Mac)

select(2) — Linux manual page: https://man7.org/linux/man-pages/man2/select.2.html

poll vs select vs event-based: https://daniel.haxx.se/docs/poll-vs-select.html

Internet Relay Chat Protocol Documentation: https://dd.ircdocs.horse/refs/commands/nick
