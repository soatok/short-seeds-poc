# Ed25519 Short Seeds Exploit Proof of Concept

In January 2025, I wrote [a blog post criticizing Session](https://soatok.blog/2025/01/14/dont-use-session-signal-fork/)
(a fork of Signal) for using 128-bit seeds with libsodium's `crypto_sign_seed_keypair()`, even though it asks for 
256-bit seeds.

This reduces the multi-user security of Ed25519. As a result, the cost of a batch attack is realistically attainable for
nation-state level attackers. 

Of course, I am not a nation-state level attacker. Thus, my proof-of-concept will be scaled down.

**[Start Here](exploit/demo1)**

## What Does This Do?


