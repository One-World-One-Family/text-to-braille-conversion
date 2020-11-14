## Introduction

These are small python scripts which helps converting txt files to converted braille txt files and vice versa

## Steps to Run

1. Clone the repository. 
2. make sure you have python3 installed

**Command to run :**

**Usage:**
python main.py ****<parameter>**
python main.py **<file name> <parameter>**

**Parameters**:
--braille | -b translate braille to text
--text | -t translate text to braille
--help | -h display this screen
--map | -m print translation map

## The Algorithmic approach

1. Split up the text into words by dividing them based on spaces and new lines (' '),('\n').
2. For each word, handle the numbers first.
    - first 10 letters of the alphabets have same braille characters as numbers in braille
    - to differentiate between digits and alphabets (⠼) character is placed before the group of numbers.
3. As numbers have prefix character same is the case with capitals with each capital letter (.) this character is added in the beginning.
4. All the punctuation surrounding the word is removed and stored. 
5. Seeing if a trimmed word can be contracted as some words for instance 'the' , 'in' etc are represented by 1 braille character.
    - translating the remaining alphabets
    - translating the stored punctuations.

### Exceptions

- There is no braille symbol for a generic quote (").
- There is only open quotation (“) and closed quotation (”).

## Steps to contribute

Everyone is welcome to contribute. 

1. just Add your name to the OWOF contributor list and you can start contributing. 
2. You can either work on an open issue or open an issue and work on it. 
3. issues can also be discussed on our Zulip Channel.

***PS**: This code might not be 100% accurate and could only be able to provide a rough conversion. please raise issues for corrections.*
