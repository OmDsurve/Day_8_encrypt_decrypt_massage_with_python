# Day_8_encrypt_decrypt_massage_with_python
This project implements the Caesar cipher, a basic encryption technique, in Python. The Caesar cipher is a form of substitution cipher where each letter in the plaintext is shifted a certain number of places down or up the alphabet. This project allows users to both encrypt (encode) and decrypt (decode) messages by specifying the shift value.

 Components:

1. Alphabet List:
   - The project uses a predefined list of alphabet letters (`alphabet`) to facilitate the shifting process. This list is essential for mapping each letter to its corresponding shifted position.

2. Caesar Function:
   - The core logic of the cipher is handled by the `caesar` function, which accepts three arguments: `original_text`, `shift_amount`, and `encode_or_decode`.
   - If the user chooses to decode a message, the function inverts the shift by multiplying the `shift_amount` by -1. This reversal allows the function to work for both encryption and decryption with the same code.
   - The function iterates through each letter in the `original_text`. For alphabetic characters, it calculates their new position by adding the `shift_amount` to their index in the `alphabet` list. The modulo operation ensures that the shifting wraps around the alphabet if necessary. Non-alphabet characters, such as spaces or punctuation, are directly appended to the output without modification.
   - The function then prints the encoded or decoded result.

3. User Interaction:
   - The program starts by displaying an ASCII art logo from the `art` module, creating an engaging introduction to the cipher tool.
   - It then enters a loop where the user is prompted to choose between encoding or decoding a message, input their text, and specify the shift value.
   - The `caesar` function processes the input, and the result is displayed to the user.
   - After each operation, the user is asked if they want to continue. If the user decides to stop, the loop ends, and the program displays a "Goodbye" message.

Learning Outcomes:
   
This project is an excellent exercise in understanding basic cryptography concepts and practicing fundamental Python skills. It reinforces knowledge of strings, loops, conditionals, and user input handling. The use of a modular approach with the `caesar` function makes the code more organized and easier to understand. Additionally, the project introduces the idea of simple encryption and decryption, which can be foundational for more advanced cryptographic techniques.
