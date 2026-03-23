picoCTF - Bytemancy-1

What I did:
- ASCII decimal 101 = 'e' (0x65)
- Challenge wants 1751 'e's side-by-side, no spaces
- Generated with Python: (b'\x65' * 1751).decode()
- Piped to nc foggy-cliff.picoctf.net 49300 → flag!

Flag: picoCTF{h0w_m4ny_e's???_7dbc095c}
