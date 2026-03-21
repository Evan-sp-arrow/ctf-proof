picoCTF - Nice netcat...

What I did:
- Connected to the challenge service using netcat (nc)
- Received a sequence of decimal ASCII numbers printed by the server
- Converted those numbers from decimal to ASCII text to reveal the flag

Commands used:
- nc wily-courier.picoctf.net 60017
- Used online decimal-to-ASCII converter or Python to decode the numbers

Flag format: picoCTF{...}
