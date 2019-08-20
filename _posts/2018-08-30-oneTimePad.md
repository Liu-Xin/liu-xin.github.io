---
title: One Time Pad
date: 2018-08-30
categories:
- technical
---

This blog post is just to go over what I learned in my first lecture of Purdue's CS355: Intro to Cryptography course.

#### How it works
Our instructor first introduced us to One Time Pad, or as he described it, an uncrackable cryptographic algorithm. Naturally, we were all shocked upon hearing this (how could this be true, our entire course summarized in one algorithm!), but as we learned more about it, we learned that the underlying concepts of One Time Pad is surprisingly simple.

Firstly, I should define the field of cryptography: the study of techniques for secure communication in the presence of third parties. If a third party obtains an encrypted message, then they should not obtain any more knowledge to the message's actual meaning compared to what they knew prior to receiving the encrypted message.

One Time Pad is one algorithm to obtain this. It provides the benefit to having an uncrackable message, at the cost of two prerequisites:
1. The sender and receiver must meet in person to generate the secret key.
2. The secret key can only be used once.
Firstly, I would meet the president of the US and generate a random bit string, {0,1}^n. Then we would part ways. So then, both me and the president would both have the secret key.

So now, back in my home, I want to send the string "Hello" to the POTUS. "Hello" converted from ASCII to bit string has a length of 40. So we will use the first 40 characters of the secret key. To generate the encrypted message, we take the bit string representing "Hello", and do XOR operation with the secret key. As long as the secret key was truly generated randomly, then the encrypted message should be safe.

When the POTUS receives the message, they decrypt it using the same 40 characters of the secret key. To decrypt, he would just XOR the encrypted message with the inverse of the secret key. Because of the XOR operations, the president would then receive the original message of "Hello".

#### Some downsides of One Time Pad
- Generating perfectly random keys are hard. Software generators sometimes repeat values + have biases. The security of One Time Pad, considering the key is only known by the sender and receiver, completely depends on the random secret generator.
- Secret keys can only be used once. If used consecutively, the middleman can deduce the key from the frequencies of bits and frequencies of alphabet, or other patterns.

#### Some benefits of One Time Pad
- the XOR operation has no bitskew and has equally probable outputs for any given input.
- the algorithm is relatively easy to implement.

I felt like going over this was a really good introduction to cryptography. It really sparked my interest in the subject and the underlying mathematics.

- Andrew