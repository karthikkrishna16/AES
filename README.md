# EX-8-ADVANCED-ENCRYPTION-STANDARD ALGORITHM

## NAME : KARTHICK KRISHNA
## REG NO : 212223240067

# Aim:
To use Advanced Encryption Standard (AES) Algorithm for a practical application like URL Encryption.

# ALGORITHM:
AES is based on a design principle known as a substitution–permutation.
AES does not use a Feistel network like DES, it uses variant of Rijndael.
It has a fixed block size of 128 bits, and a key size of 128, 192, or 256 bits.
AES operates on a 4 × 4 column-major order array of bytes, termed the state

# PROGRAM:
```
def xor_encrypt_decrypt(input_text, key):
    input_len = len(input_text)
    key_len = len(key)
    result = ''.join([chr(ord(input_text[i]) ^ ord(key[i % key_len])) for i in range(input_len)])
    return result


if __name__ == "__main__":
    url = input("Enter the text: ")
    key = "secretkey"

    print("Original text:", url)

   
    encrypted_text = xor_encrypt_decrypt(url, key)
    print("Encrypted text:", encrypted_text)

  
    decrypted_text = xor_encrypt_decrypt(encrypted_text, key)
    print("Decrypted text:", decrypted_text)

```
# OUTPUT:

![CRY 8](https://github.com/user-attachments/assets/3666a444-68a0-4d6b-9bd9-8d569ba81a7f)


# RESULT:

THE EXPERIMENT IS EXECUTED SUCCESSFULLY
