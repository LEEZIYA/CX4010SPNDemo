# CX4010 Project: Demonstration of Attacks on SPN Ciphers
Team member: Hu Zhuangyu, Li Ziyang
##I. Overview
Construct a simple SPN implementation and apply differential and linear cryptanalysis attack on the cipher to extract the key
##II. SPN cipher
SPN cipher is a type of block cipher. It combines substitution boxes (s-box) and permutation boxes (p-box) for multiple rounds to achieve confusion and diffusion. A key scheduling algorithm is used to generate sub keys for each round of scrambling. Recovring the key is difficult even when both the plaintext and ciphertext are know (chosen plaintext attack).

##II. Differential Cryptanalysis
Differential Cryptanalysis is a type of known plaintext attack that was first published by Biham and Shamir in 1993. It was used to attack DES and other similar block ciphers. It involves using specially constructed pairs of plaintext with known difference to observe pattern in the ciphertext and extract the key.

#III. Linear Cryptanalysis
Linear Cryptanalysis is a technique first published by Mitsuru Matsui in 1992.

