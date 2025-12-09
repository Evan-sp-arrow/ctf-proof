picoCTF - Magikarp Ground Mission

What I did:
- Launched the challenge instance on picoCTF to get SSH host, port, username, and password
- Used ssh to connect as ctf-player to the given host and port
- Listed files and read 1of3.flag.txt to get the first part of the flag
- Read instructions-to-2of3.txt which told me to go to the root directory '/'
- At '/', read 2of3.flag.txt and instructions-to-3of3.txt for the next location
- Followed the instructions to the final directory, read 3of3.flag.txt, and concatenated all three parts into one picoCTF{...} flag

Commands used (high level):
- ssh ctf-player@<host> -p <port>
- ls, cd, cat
