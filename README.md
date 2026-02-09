# IT16FirstLabExam
## How Encryption and Decryption Works

Encryption follows the formula `E = (X + N) % 26`, where X represents the letter's position in the alphabet (A=0, B=1, etc.) and N is the shift number. This process shifts each letter forward by N positions, wrapping around to the start of the alphabet when reaching Z using modulo 26. For example, with a shift of 3, A becomes D, B becomes E, and so on.

Decryption uses the inverse formula `D = (X - N) % 26`, which reverses the encryption by shifting each letter backward by N positions. The same modulo 26 ensures proper wrapping from A back to Z. For instance, with a shift of 3, D returns to A, E returns to B, maintaining the exact reverse operation of encryption.

The algorithm processes each character individually, converting uppercase letters (A-Z) using ASCII values starting from 65, and lowercase letters (a-z) starting from 97. Numbers, spaces, and symbols remain unchanged throughout both encryption and decryption, preserving the original format while only transforming the alphabetic characters according to the specified mathematical formulas.
