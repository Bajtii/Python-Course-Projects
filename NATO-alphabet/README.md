# 🔤 NATO Phonetic Alphabet Converter

A simple Python program that converts a user-inputted word into the NATO phonetic alphabet using a CSV file as a source. It's a practical exercise for working with `pandas`, dictionary comprehensions, and user interaction in Python.

## 📋 Description

This program reads a CSV file (`nato_phonetic_alphabet.csv`) containing the NATO phonetic alphabet (e.g., A = Alpha, B = Bravo, etc.) and then:

1. Creates a dictionary mapping each letter to its corresponding code word.
2. Prompts the user to enter a word.
3. Converts each letter of the word to its phonetic code equivalent.
4. Outputs the result as a list of phonetic words.

## 🗂️ Example CSV File Format

**nato_phonetic_alphabet.csv**
```csv
letter,code
A,Alpha
B,Bravo
C,Charlie
...
Z,Zulu
```
