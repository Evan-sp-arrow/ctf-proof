picoCTF - Information (Metadata)

What I did:
- Ran exiftool on cat.jpg → found base64 flag in License field
- Extracted with grep + sed → decoded with base64 -d

Commands:
exiftool cat.jpg | grep License | sed -e 's/.*: //' | base64 -d

Flag: picoCTF{the_m3tadata_1s_modified}
