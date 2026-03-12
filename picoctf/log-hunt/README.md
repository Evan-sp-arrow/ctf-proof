picoCTF - Log Hunt

What I did:
- Downloaded server.log from the challenge
- Used grep to find all lines containing "FLAGPART"
- Extracted the 4 unique flag pieces using sed, awk, tr
- Assembled them in timestamp order into the full flag

Commands used:
- grep "FLAGPART" server.log
- grep "FLAGPART" server.log | sed "s/.*FLAGPART: //" | awk "!seen[$0]++" | tr "
" "_" | sed "s/_$//"
