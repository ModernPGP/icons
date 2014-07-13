Icons
=====

A collection of icons representing PGP's implementation in graphical interfaces


Projects
========
[Mailpile](https://github.com/pagekite/Mailpile), [OpenKeychain](https://github.com/open-keychain/open-keychain), [GPGTools](https://github.com/GPGTools)


Signature States
================

Here are the signature state names + description that Mailpile is currently using.


#### Not Signed
This message contains no signature, which means it could have come from anyone, not necessarily the real sender


#### Invalid
The signature was invalid or bad


#### Revoked
Watch out, the signature was made with a key that has been revoked- this is not a good thing


#### Expired
The signature was made with an expired key

#### Unknown
The signature was made with an unknown key, so we can not verify it


#### Unverified
The signature was good but it came from a key that is not verified yet


#### Verified
The signature was good and came from a verified key, w00t!


#### Error
There was a weird programatic error trying to analyze this signature
