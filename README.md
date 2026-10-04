# Encrypted handoff

This repository contains an encrypted archive. The recipient private key is
required and is not included. Install age from https://github.com/FiloSottile/age.

Decrypt and extract locally:

```sh
age --decrypt -i recipient-key.txt -o payload.tar.xz payload.age
tar -xf payload.tar.xz
```

The archive contains its own instructions and file checksums. Do not commit the
private key or decrypted output into this public repository.
