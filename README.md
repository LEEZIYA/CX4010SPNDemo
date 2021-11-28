# CX4010 Project: Demonstration of Attacks on SPN Ciphers
Team member: Hu Zhuangyu, Li Ziyang

## Overview
Construct a simple SPN implementation and apply linear cryptanalysis attack on the cipher to extract the key

## Motivation
SPN cipher is a type of block cipher. It combines substitution boxes (s-box) and permutation boxes (p-box) for multiple rounds to achieve confusion and diffusion. A key scheduling algorithm is used to generate sub keys for each round of scrambling. Recovring the key is difficult even when both the plaintext and ciphertext are know (chosen plaintext attack). 

Linear Cryptanalysis, first published by Mitsuru Matsui in 1992, is one of the two important techniques for cryptoanalysis (the other one is differential cryptoanalysis). It involves constructing linear eauqtions to approximates the relationship between and using the equation 

## Research & Design
We implement a simple SPN with 2 rounds of 4x4 bit S-boxes and 8 bit p-boxes, with fixed mapping for the s-boxes and p-boexes. 8 bit plaintext and key is used. Key is generated randomly using os.urandom module. A simple key extension algorithm is used to generate two round keys from the key.
We implement the linear cryptanalysis with reference to a tutorial by Howard M. Heys (https://ioactive.com/wp-content/uploads/2015/07/ldc_tutorial.pdf) and a github repository (https://github.com/physics-sec/Linear-Cryptanalysis)

## Development
All codes are written in Python language in one single Python jupyter notebook file with comments and markdowns. An OOP designed SPN is developed and tested before applying linear cryptanalysis. For demonstration, run the SPN_Network.ipynb from the top using Jupyiter Notebook or google colab. Alternatively, run the SPN_Network.py file using python intepreter or IDE. The two file have same content.

## Use of the Code
The codes may be used for linear cryptanalysis of SPN ciphers


