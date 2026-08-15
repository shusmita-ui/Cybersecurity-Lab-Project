# Cryptography Basics


## Objective


To understand the basic concepts of encryption, hashing, digital certificates, SSL/TLS, and practical cryptographic operations using OpenSSL.


---


## 1. Symmetric Encryption


Symmetric encryption uses the same secret key for both encryption and decryption.


### Example


AES (Advanced Encryption Standard)


### Advantages


- Fast encryption and decryption
- Suitable for encrypting large amounts of data
- Requires less computational power


### Disadvantage


The secret key must be securely shared between the communicating parties.


---


## 2. Asymmetric Encryption


Asymmetric encryption uses two different but mathematically related keys:


- Public Key
- Private Key


The public key can be shared, while the private key must be kept secret.


### Examples


- RSA
- ECC


### Uses


- Secure key exchange
- Digital signatures
- Authentication
- Digital certificates


---


## 3. AES


AES stands for Advanced Encryption Standard.


AES is a symmetric block cipher commonly used to protect sensitive data.


The laboratory included an AES encryption and decryption practical using OpenSSL.


### Basic Concept


```text
Plaintext
    ↓
AES Encryption + Secret Key
    ↓
Ciphertext
    ↓
AES Decryption + Secret Key
    ↓
Original Plaintext
4. Hashing

Hashing converts input data into a fixed-length hash value.

Hashing is a one-way operation and is mainly used for data integrity verification.

MD5

MD5 produces a 128-bit hash value.

Example:

md5sum file.txt
SHA-256

SHA-256 produces a 256-bit hash value.

Example:

sha256sum file.txt

SHA-256 is generally preferred over MD5 for modern security applications.

5. Encryption vs Hashing
Feature	Encryption	Hashing
Purpose	Protect data confidentiality	Verify data integrity
Reversible	Yes, with the correct key	No
Key required	Usually yes	No
Example	AES	SHA-256
6. Digital Certificates

A digital certificate is used to associate a public key with an identity.

X.509 certificates are commonly used with SSL/TLS.

A self-signed X.509 certificate was generated during the laboratory exercise.

Certificate Information

The certificate contained information such as:

Country
State
Locality
Organization
Common Name
Public key
Validity period
7. SSL/TLS

TLS (Transport Layer Security) provides secure communication over a network.

TLS provides:

Confidentiality
Authentication
Integrity

HTTPS uses TLS to protect web communication.

8. OpenSSL

OpenSSL is a cryptographic toolkit used for:

Encryption
Decryption
Hashing
Key generation
Certificate generation
TLS testing
Check OpenSSL Version
openssl version
Generate RSA Private Key
openssl genrsa -out server.key 2048
Generate a Self-Signed Certificate
openssl req -new -x509 -key server.key -out server.crt
9. Practical Work

The following cryptography activities were performed:

AES encryption
AES decryption
MD5 hashing
SHA-256 hashing
RSA key generation
X.509 certificate generation
SSL/TLS testing
OpenSSL command-line operations