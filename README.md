# Decypher
A CLI for speedy Cipher Decryption/Encryption

![image](https://github.com/Aswinr24/Decypher/assets/135364633/fa60340a-d339-4846-b861-49b7082c205e)

![image](https://github.com/Aswinr24/Decypher/assets/135364633/f08b6499-ff46-4f6f-b7d0-0093cb798049)


### Installation:
#### Python:
```
pip install decypher
```
#### Docker:
Pull the docker image:
```
docker pull aswinr24/decypher:decypher
```
Run the Container: 
```
docker run -it --rm decypher
```

### Usage:

To see the list of available ciphers for encryption/decryption and options:
```
decypher --help
```
To decrypt a Cipher:
```
decypher 'Ciphername' 'Ciphertext' 'key(based on type of cipher)'
```
To encrypt plaintext as a Cipher:
```
decypher 'Ciphername' 'Ciphertext' 'key' --encrypt
```
To view the version:
```
decypher -v
```

Using Docker:
```
docker run -it --rm decypher <Ciphername> <CipherText/Plaintext> <key>
```
Replace `<Ciphername>` with the name of the Cipher, `<Ciphertext/Plaintext>` with the Ciphertext or Plaintext to encrypt/decrypt and `<key>` with the key.
