# Generating a private key
`openssl genrsa -out privkey.pem 2048`

# Getting public key from private key
`openssl rsa -in privkey.pem -pubout -out pubkey.pem`