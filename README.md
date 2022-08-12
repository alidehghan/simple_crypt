# Simple Crypt

A simple and high level rust library to encrypt and decrypt text, files and any data with it

For encryption it uses [AES-GCM-SIV-256](https://en.wikipedia.org/wiki/AES-GCM-SIV) and [Argon2](https://en.wikipedia.org/wiki/Argon2)

## Usage

add this to Cargo.toml:

```toml
simple_crypt = "*"
```

## Examples

Encrypting

```rust
let encrypted_data = encrypt(b"example text", b"example passowrd").expect("Failed to encrypt");
```

Decrypting

```rust
let data = decrypt(&encrypted_data, b"example passowrd").expect("Failed to decrypt");
```

And there are other functions to encrypt files or folders see the [documentation](https://docs.rs/simple-crypt)

Go to [Documentation](https://docs.rs/simple-crypt) | [Repository](https://github.com/NiiightmareXD/simple_crypt)
