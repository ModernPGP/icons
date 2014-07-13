Icons
=====

A collection of icons representing PGP's implementation in graphical interfaces. Icons are grouped together according to Encryption, Key, and Signature.


Projects
========

* [Mailpile](https://github.com/pagekite/Mailpile) - a Free / open source fast modern webmail client
* [OpenKeychain](https://github.com/open-keychain/open-keychain)
* [GPGTools](https://github.com/GPGTools)


Encryption
==========

#### Open

The open lock icon SHOULD be used to represent a message or data that is going to be sent "unencrypted"

![Unncrypted Icon](https://raw.githubusercontent.com/ModernPGP/icons/master/encryption/lock-open.png)


#### Closed

The closed lock icon is used to represent data that WAS encrypted but HAS BEEN successfully decrypted or used for outgoing message or data that WILL BE encrypted.

![Encrypted Icon](https://raw.githubusercontent.com/ModernPGP/icons/master/encryption/lock-closed.png)


#### Error

The error lock icon represents data that IS encrypted and COULD NOT be decrypted.

![Error Icon](https://raw.githubusercontent.com/ModernPGP/icons/master/encryption/lock-error.png)


Keys
====

#### Fingerprint
Use this icon to represent fingrprint of a PGP key

![Fingerprint Icon](https://raw.githubusercontent.com/ModernPGP/icons/master/keys/icon-fingerprint.png)

#### Key
Use this icon to represent a PGP key or Key ID 

![Key Icon](https://raw.githubusercontent.com/ModernPGP/icons/master/keys/icon-key.png)


Signatures
==========

Here are the signature state names + description that Mailpile is currently using.


#### Invalid
The signature was invalid or bad

![Invalid Signature Icon](https://raw.githubusercontent.com/ModernPGP/icons/master/signatures/signature-invalid-cutout.png)


#### Revoked
Watch out, the signature was made with a key that has been revoked- this is not a good thing

![Revoked Signature Icon](https://raw.githubusercontent.com/ModernPGP/icons/master/signatures/signature-revoked-cutout.png)


#### Expired
The signature was made with an expired key

![Expired Signature Icon](https://raw.githubusercontent.com/ModernPGP/icons/master/signatures/signature-expired-cutout.png)


#### Unknown
The signature was made with an unknown key, so we can not verify it

![Unknown Signature Icon](https://raw.githubusercontent.com/ModernPGP/icons/master/signatures/signature-unknown-cutout.png)


#### Unverified
The signature was good but it came from a key that is not verified yet

![Unverified Signature Icon](https://raw.githubusercontent.com/ModernPGP/icons/master/signatures/signature-unverified-cutout.png)


#### Verified
The signature was good and came from a verified key, w00t!

![Verified Signature Icon](https://raw.githubusercontent.com/ModernPGP/icons/master/signatures/signature-verified-cutout.png)


#### Error
This state exists when there was a weird programatic error trying to analyze this signature. There is no icon for this state

#### None
This state exists when there was no signature. There is no icon for this state.


QR Code
=======
* monkeysphere URI scheme is ugly: ``openpgp4fpr:73EE2314F65FA92EC2390D3A718C070100012282``
* ``openpgp4fpr`` makes no sense

our proposal: ``pgp-fingerprint:73EE2314F65FA92EC2390D3A718C070100012282``  
optional parameters:
* ``name``
* ``address`` (e.g. email, jabber)
* ``url``
* ``keyserver``

Example: ``pgp-fingerprint:73EE2314F65FA92EC2390D3A718C070100012282?keyserver=hkp://pool.skskeyservers.net&address=dominik@dominikschuermann.de&url=http://sufficientlysecure.org&name=Dominik``
