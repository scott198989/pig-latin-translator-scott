## PLAN
For functionality we need to break up the words into parts, the prefix, suffix, and index.  We can use the eachWord.slice method to turn each word into seperate strings of letters starting at the 0 index.  

We need to segment each question into its own statement in the else if statement.  

We begin with the vowelsArray in the if statement and iterate over the entire length and if the length of the array strictly has no remainder, or has no vowels "ay" will be added to the end of eachWord by using += "ay".

If that condition is not met, we will else if and iterate over the entire vowelsArray and use the .includes method to look for the letter "u".  If the inputed word has the letter "u" AND the letter "q" we can use .includes and .indexOf methods to move the q and the u, but we have to seperatley idenfiy them and include the logical and (&&).

If none of those conditions are met our catch all will be to move the first consonants to the end of the word and add "ay" by using the .indexOf to find the first letter at the zero index, slicing the word into seperate strings, slicing the index, and adding the suffix and prefix and adding the "ay".  

One big else if statement.

---

STUDENT NOTES ABOVE

![Pig Latin Translator Screenshot](https://github.com/scott198989/pig-latin-translator-scott/blob/main/Piglatin-screenshot.png)

# Pig Latin Translator 🐷

## Table of Contents

- [Introduction](#introduction)
- [How it Works](#how-it-works)
- [Features](#features)
- [Dependencies](#dependencies)
- [Installation](#installation)
- [Contact](#contact)

## Introduction

Ever wanted to speak Pig Latin but didn't want to do the mental gymnastics? Well, here's your solution. This Pig Latin Translator was one of the first projects I tackled at LEARN Academy, and it uses React state to translate words or phrases into Pig Latin.

## How it Works

Under the hood, the app segments each word into a prefix, suffix, and index. Then, based on a series of conditions like whether the word contains vowels or certain consonants, it rearranges the word according to Pig Latin rules. It's basically one big `else-if` statement taking care of all the logic. Want to know more? Check out the code!

## Features

- Translate a single word or a whole phrase into Pig Latin
- Instant translation after you hit 'Submit'
  
## Dependencies

**Software Needed**

- [Homebrew](https://brew.sh/)
- [Yarn](https://yarnpkg.com/)

## Installation

1. Update Homebrew:
    ```bash
    brew update
    ```
2. Install Yarn:
    ```bash
    brew install yarn
    ```
3. Run Locally
   ```bash
   yarn
   yarn start
   ```

## Contact

If you dig this project or just want to say hi, feel free to hit me up on [LinkedIn](https://www.linkedin.com/in/scott-tuschl). You can also find more of my work at my [portfolio site](https://www.scott-tuschl.com).
