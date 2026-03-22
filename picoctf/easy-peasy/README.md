picoCTF - Easy Peasy (Broken OTP)

What I did:
- Connected with nc wily-courier.picoctf.net 64002
- Flag encrypted: 73e7a714676a81d9bd03339392733c7af01ccb2cdd9dd3d0dac14f90655b79db (32 bytes)
- Sent 49968 'a's + 32 'a's to reset key position to 0 (KEY_LEN=50000)
- Got encryption of 32 'a's using same key as flag
  print('{:x}'.format(ef^ea^pa))
# Output: 6662393734386139373863316666366531613863666635633465636433373738

# Convert hex → ASCII:
# https://www.rapidtables.com/convert/number/hex-to-ascii.html
# Paste: 6662393734386139373863316666366531613863666635633465636433373738
# Result: fb978a978c1f6e1a8cff5c4ecd3778 → picoCTF{...} 
Flag: picoCTF{fb978a978c1f6e1a8cff5c4ecd3778}
