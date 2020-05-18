---
title: Introduction
menu: true
order: 1
---

# Simple, Fast, Secure.
BI-SGX is one of the most practical solutions for cloud secret computation. You can easily execute secret computation on cloud with utilizing fast processing speed and high security of Intel SGX.

![photo](/assets/img/BISGX_overview.png)

By using BI-SGX, you don't have to use infamous SGXSDK anymore! BI-SGX provides original simple and clear language named Qliphoth.  

Comparing with fully-homomorphic encryption (FHE), the most famous existing methods for secret computation, BI-SGX can execute secret computation extremely faster than FHE.

![photo](/assets/img/compare.png)

BI-SGX mainly provides secret computation features for bioinformatic analysis, but you can easily apply BI-SGX for more generic computations.

# Qliphoth - brand-new simple and secure language
![photo](/assets/img/Qliphoth_logo.png)

Are you disgusted with SGXSDK? Extremely complicated SGXAPI, redundant unique types, EDL, implicit specifications, Bloat of source codes... As you know, SGXSDK is **inhumane**.  

Do you know this report about code bloat by modifying legacy program to SGX-capable one? The paper of [SgxElide](https://web.cse.ohio-state.edu/~lin.3021/file/CGO18.pdf) says that when they modified 412 LOC legacy program to SGX-capable code, the deliverable became **3523 LOC**.

![photo](/assets/img/codeBloat.png)

As you can see, SGXSDK is really inhumane architecture. To save developers from the clutches of the SGXSDK, BI-SGX provides brand-new interpreter language called Qliphoth.

## Easy to use
The grammar of Qliphoth is really clear like Python and Ruby. Qliphoth also provides various built-in functions for math, RNG and bioinformatics. You don't need to implement any trivial SGX-related processes like enclave initialization, Remote Attestation, EDL, dividing large data into EPC-suitable size, etc. Only you have to write is what you want to compute inside the enclave.

![photo](/assets/img/qli_ex.png)

## Protect output privacy
Qliphoth is designed to solidly protect output privacy of secret data. When a code follows a protocol but output results which violates privacy, we say it violates output privacy; And such codes are called **semi-honest**.   

For example, obtaining average of single value follows its protocol (the protocol means calculating average using provided function here), but it outputs the secret data itself.  

Qliphoth prevents such semi-honest operation, therefore Qliphoth is secure language and suitable for cloud secret computing.

## Why you named "Qliphoth"?

# Protection against side-channel attacks

# Deploy on your public cloud instance

# Package image

# MITOU 2019, IPA
