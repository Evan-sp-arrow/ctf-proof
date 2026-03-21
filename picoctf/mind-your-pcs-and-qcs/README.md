picoCTF - Mind your Ps and Qs (RSA Decryption)

What I did:
- Used factordb.com to factor n into primes p and q
- Computed phi(n) = (p-1)*(q-1)
- Found private key d = e^-1 mod phi(n)
- Decrypted ciphertext c^d mod n → hex → bytes → reverse → flag

Given values:
- c: 15341890103764929939105506004034128738090325640037083301857608662849501626260517
- n: 948406957756830799684818171639547165784816468744946013083947881743680617123566349
- e: 65537

Factored using factordb:
- p: 1891771437429478964908181306574287207137
- q: 501332739776173570344039681219489434626477

Flag: picoCTF{sma11_N_n0_g0od_1dc7ae91}
