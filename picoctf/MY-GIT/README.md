picoCTF - MyGit (Git Author Impersonation)

What I did:
- Cloned challenge git repo over SSH
- Changed git config to user.name="root" and user.email="root@picoctf"
- Created flag.txt and committed as root:root@picoctf
- Pushed → server checked author match + flag.txt → gave flag

Key insight: Server only checks git commit author, not authentication!

Flag: picoCTF{1mp3rs0n4t4_g17_345y_367122f4}
