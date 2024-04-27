# Decypher

[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
![PyPI - Python Version](https://img.shields.io/pypi/pyversions/decypher?color=green)
[![PyPI version](https://img.shields.io/pypi/v/decypher.svg?color=yellow)](https://pypi.org/project/decypher/)
[![License: MIT](https://img.shields.io/badge/License-MIT-red.svg)](https://opensource.org/licenses/MIT)



A CLI for speedy Cipher Decryption/Encryption

![image](https://github.com/Aswinr24/Decypher/assets/135364633/fa60340a-d339-4846-b861-49b7082c205e)

![image](https://github.com/Aswinr24/Decypher/assets/135364633/f08b6499-ff46-4f6f-b7d0-0093cb798049)


## Installation:
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

## Usage:

To see the list of available ciphers for encryption/decryption and options:
```
decypher --help
```
To decrypt a Cipher:
```
decypher <Ciphername> <Ciphertext> <key(based on type of cipher)>
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
Replace `<Ciphername>` with the name of the Cipher, `<Ciphertext/Plaintext>` with the Ciphertext or Plaintext to encrypt/decrypt and `<key>` with the key, use `--encrypt` flag at the end for Encryption.

### Examples:

Encrypt a message using the Caesar Cipher:
```
decypher ceaser <Plaintext> <Key> --encrypt
```
Decrypt a Rail-fence Cipher:
```
decypher rail-fence <CipherText> <Key>
```
Decrypt a Vignere Cipher(using docker):
```
docker run -it --rm decypher vignere <Ciphertext> <Key>
```

## Contributing

Contributions are welcome! If you find any bugs or have suggestions for improvements, please open an issue or clone the repository and submit a pull request on GitHub.

## License

This project is licensed under the MIT License - see the [MIT License](LICENSE) file for details.
