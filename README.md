# RSA-crypto

# Dependancies
Python standard library
Python 3.5+
# Installation
Copy file into python library folder or work folder
# Usage
First run `import rsa_crypto`
You will need a private and public key pair. This can be obtained by yourself or by using this library
```
rsa_crypto.genkeypair(p,q) -> (pubkey, prvkey, n)
```
Then you can go ahead and start encrypting and decrypting messages.
```
rsa_crypto.encrypt(message, pubkey, n) -> encrypted message
```
Here message is an int, pubkey is an int and n is an int. Encrypted message is a string.

```
rsa_crypto.decrypt(encrypted, prvkey, n) -> message
```
Here encrypted is an int, prvkey is an int and n is an int. message is a string.

To convert a message to an int, use:
```
rsa_crypto.str2int(string) -> [int,int,int...]
```
To convert a list of ints back to strings, usse:
```
rsa_crypto.int2str
```
