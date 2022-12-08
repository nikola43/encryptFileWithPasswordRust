# How to securely encrypt a file with an password in Rust (using Streaming Encryption + Argon2)

## Usage

```bash
$ cargo run -- file.txt
$ cargo run -- file.txt.encrypted
```

## Check
```bash
$ shasum -a 256 file.txt file.txt.encrypted file.txt.decrypted
```

60cadf0373cb3c7c1ad77b1e327ea2fc70500f035d8f718698844ff26aa9d084  file.txt
accdb29c5904c4f76f4360df3c4618640cdfced749a34c605311100716e6f9c0  file.txt.encrypted
60cadf0373cb3c7c1ad77b1e327ea2fc70500f035d8f718698844ff26aa9d084  file.txt.decrypted