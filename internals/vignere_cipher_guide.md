# Vigenère Cipher Guide

The **Vigenère cipher** is a method of encrypting text using a **keyword**.

Unlike a simple substitution cipher, the same letter can be encrypted differently depending on its position and the key.

## How It Works

Choose a message and a keyword.

```text
Message:  ATTACKATDAWN
Key:      LEMON
```

Repeat the key until it matches the length of the message:

```text
Message:  ATTACKATDAWN
Key:      LEMONLEMONLE
```

Each letter is shifted according to the corresponding letter of the key.

Using the standard Vigenère table:

```text
        A B C D E F G H I J K L M N O P Q R S T U V W X Y Z
A       A B C D E F G H I J K L M N O P Q R S T U V W X Y Z
B       B C D E F G H I J K L M N O P Q R S T U V W X Y Z A
C       C D E F G H I J K L M N O P Q R S T U V W X Y Z A B
...
```

The row is determined by the **key letter**, while the column is determined by the **message letter**.

### Example

To encrypt:

```text
Message: A
Key:     L
```

Find row `L` and column `A`.

The result is:

```text
L
```

Another example:

```text
Message: T
Key:     E
```

Row `E`, column `T` gives:

```text
X
```

Repeating this process produces the encrypted message.

---

## Decryption

To decrypt a Vigenère message, use the same keyword.

Instead of shifting forward, shift **backward** according to the key.

For example:

```text
Ciphertext: LXFOPV
Key:        LEMONL
```

Decrypting it produces:

```text
ATTACK
```

---

## Important Rules

- Remove spaces and punctuation when applying the cipher, unless the puzzle specifies otherwise.
- Repeat the keyword for the entire message.
- The **keyword is required** to decrypt the message.
- Different keywords produce completely different results.
- The key is usually a word or short phrase.

## Quick Reference

Assign each letter a value:

```text
A = 0
B = 1
C = 2
D = 3
...
Z = 25
```

For encryption:

```text
Cipher = (Message + Key) mod 26
```

For decryption:

```text
Message = (Cipher - Key) mod 26
```

**If a recovered message appears to be encrypted but does not respond to simple substitution or Caesar shifts, a keyword-based cipher may be worth investigating.**
