alphabet = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z']

direction = input("Type 'encode' to encrypt, type 'decode' to decrypt:\n")

def encrypt(plain_text, shift_amount):
  encrypted_word = ""
  for letter in text:
    if letter == " ":
      encrypted_word += " "
    elif(alphabet.index(letter) + shift < len(alphabet)):
      encrypted_word += alphabet[alphabet.index(letter) + shift]
    else:
      index = alphabet.index(letter) + shift - len(alphabet)
      encrypted_word += alphabet[index]
  print(f"The encoded text is {encrypted_word}")

def decrypt(plain_text, shift_amount):
  decrypted_word = ""
  for letter in text:
    if letter == " ":
      decrypted_word += " "
    elif alphabet.index(letter) - shift >= 0:
      decrypted_word += alphabet[alphabet.index(letter) - shift]
    else:
      index = alphabet.index(letter) - shift
      decrypted_word += alphabet[index]
  print(f"The encoded text is {decrypted_word}")

if direction == "encode":
  text = input("Type your message:\n").lower()
  shift = int(input("Type the shift number:\n"))
  encrypt(plain_text = text, shift_amount = shift)
elif direction == "decode":
  text = input("Type your message:\n").lower()
  shift = int(input("Type the shift number:\n"))
  decrypt(plain_text = text, shift_amount = shift)
else:
  print("Directions unclear.")

