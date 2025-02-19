The **Secure Shell Protocol (SSH Protocol)** is a super-secure way to connect to external servers.

It is a cryptographic network that enables secure communication over networks that may or may not be secure. Think of it like a tunnel from one computer to another!

ssh typically runs at TCP/IP port 22

# command

```zsh
ssh [username]@[hostname or IP]
```

typically, you are given a remote server username `[username]` to connect with a `[hostname or IP]`

## Options

Here are the command options for the `ssh` command

| Option | Description                                                                                                                                     |
| ------ | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| -1     | Forces ssh to use ssh-1 protocol only                                                                                                           |
| -2     | Forces ssh to use ssh-2 protocol only                                                                                                           |
| -4     | Allows IPv4 addresses only                                                                                                                      |
| -6     | Allows IPv6 addresses only                                                                                                                      |
| -A     | Authentication agent connection forwarding is enabled                                                                                           |
| -a     | Authentication agent connection forwarding is disabled                                                                                          |
| -C     | Compresses all data for faster transfer of data                                                                                                 |
| -c     | Selects the cipher specification for encrypting the session (specific algorithm will only be selected if both the client and server support it) |
| -f     | Requests ssh to go to background just before command execution                                                                                  |
| -g     | Allows remote hosts to connect to local forwarded ports                                                                                         |
| -n     | Prevents reading from stdin                                                                                                                     |
| -p     | Port to connect to on the remote host                                                                                                           |
| -q     | Suppresses all error and warnings                                                                                                               |
| -V     | Display the version number                                                                                                                      |
| -v     | Verbose mode, useful for debugging connection failures                                                                                          |
| -X     | Enables X11 forwarding                                                                                                                          |

# public-private keys

```zsh
ssh-keygen
```

You can set up an asymmetric key cryptographic system to connect to an SSH server. The advantage of this is that you will no longer need to use a password to `ssh` into a system.

# Acknowledgements
---
Most of this information is from GeeksForGeeks.org:
- https://www.geeksforgeeks.org/ssh-command-in-linux-with-examples/