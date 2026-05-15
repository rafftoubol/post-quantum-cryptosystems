## Features

| Feature | Status |
| :--- | :---: |
| GGH-HNF Implementation with Key Encapsulation Methods | ✅ |
| LLL Lattice Reduction for SVP Based Cryptosystem attacks | ✅ |
| Code Based Cryptosystem Implementation with real world testing for successful decryption rates based on noise (T) value | ✅ |
| NTRU Implementation | ✅ |
|  Test harness, which outputs and plots results with informative visuls| ✅ |

## Useage / Installation
The python jupyter books in this repo require a 'sagemath' kernel to properly execture, duo to specific mathematical functions.
This can be most simply achieved by running the kernel in a docker as per the info at https://www.sagemath.org/ , then pointing your IDE to the jupyter sagemath kernel served over localhost.
Once the kernel is running successfully, each section of the jupyter books are well documented, and will either output in the stdout below the cell, or generate keys / visual pdfs in subfolders

## Please dont use these for important data
1. the lattice based cryptosystems require such a large keyspace to be real world applicable in this implementation (20GB public keys)
   - GGH-HNF was one of the first algorithms, its widely considered insecure in 2026
   - NTRU is the more modern alternative, however NIST in the FIPS define a more secure extension of NTRU
2. The code based systems here leverage BCH codes as opposed to the Goppa Codes that NIST/FIPS specify, this is simply for a proof of concept.

 _This repo is simply to show the logic behind cryptosystem development, how you can test cryptosystems and create an understanding of the pipeline_ 
