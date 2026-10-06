# Hash Identification Reference

A **hash** is a fixed-length value generated from data using a hashing algorithm.

Hashes are commonly represented as hexadecimal characters.

> A hash is not the same as encryption. Hashing is generally designed to be one-way.

## Common Hash Formats

| Algorithm   | Typical Length | Hex Characters | Example                                                                                                                            |
| :---------- | -------------: | :------------: | :--------------------------------------------------------------------------------------------------------------------------------- |
| **MD5**     |       128 bits |       32       | `5d41402abc4b2a76b9719d911017c592`                                                                                                 |
| **SHA-1**   |       160 bits |       40       | `7f7e3f1b5a2d8e9c4a6b1c0d3e5f789012345678`                                                                                         |
| **SHA-224** |       224 bits |       56       | `d14a028c2a3a2bc9476102bb288234c415a2b01f828ea62ac5b3e42f`                                                                         |
| **SHA-256** |       256 bits |       64       | `9f86d081884c7d659a2feaa0c55ad015a3bf4f1b2b0b822cd15d6c15b0f00a08`                                                                 |
| **SHA-384** |       384 bits |       96       | `38b060a751ac96384cd9327eb1b1e36a21fdb71114be07434c0cc7bf63f6e1da274edebfe76f65fbd51ad2f14898b95b`                                 |
| **SHA-512** |       512 bits |      128       | `cf83e1357eefb8bdf1542850d66d8007d620e4050b5715dc83f4a921d36ce9ce47d0d13c5d85f2b0ff8318d2877eec2f63b931bd47417a81a538327af927da3e` |

## Identifying a Hash

Count the hexadecimal characters.

```text
32 characters  →  Possibly MD5
40 characters  →  Possibly SHA-1
56 characters  →  Possibly SHA-224
64 characters  →  Possibly SHA-256
96 characters  →  Possibly SHA-384
128 characters →  Possibly SHA-512
```

### Important

**Length alone does not prove which algorithm was used.**

Different hashing systems can produce values with the same length, and hashes may also be encoded or formatted differently.

## Hexadecimal Characters

A standard hexadecimal hash contains only:

```text
0 1 2 3 4 5 6 7 8 9
A B C D E F
```

For example:

```text
9f86d081884c7d659a2feaa0c55ad015a3bf4f1b2b0b822cd15d6c15b0f00a08
```

contains **64 hexadecimal characters**, making it consistent with a SHA-256 hash.

## Quick Reference

```text
MD5      = 32 hex characters
SHA-1    = 40 hex characters
SHA-224  = 56 hex characters
SHA-256  = 64 hex characters
SHA-384  = 96 hex characters
SHA-512  = 128 hex characters
```

When a long string of seemingly random hexadecimal characters is recovered, **count the characters before attempting to decode it**.

A hash generally should be **verified or compared**, rather than treated as an encoded message that can simply be decoded.
