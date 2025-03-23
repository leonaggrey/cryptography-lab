# Cryptography-lab
This repo contains decrypt.py as lab 1 and reading assignment pdf.
# Overview Lab 1 (decrypt.py)
This Python script demonstrates an attack on the one-time pad cipher when the same key is reused multiple times. By analyzing multiple ciphertexts encrypted with the same key, it attempts to recover the original plaintext messages and partially reconstruct the encryption key.

# How It Works
XOR Analysis: The script XORs different ciphertext pairs to detect probable space characters, as spaces are the most common character in natural language.

Key Recovery: Once probable spaces are identified, it attempts to derive the encryption key by assuming a space (' ') was used in plaintext.

Plaintext Recovery: Using the recovered key bytes, the script decrypts the ciphertexts, revealing portions of the original messages.

Target Message Decryption: The script attempts to decode a specific target ciphertext using the reconstructed key.
