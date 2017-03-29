Implemented an improved Secure Socket Communication protocol.

In the improved security protocol, the process is done in 3 steps.

  First, Bob generates the certificate and sends it to Alice. 
  Second, keys are exchanged between Bob and Alice. 
  Finally, data is exchanged by encrypting and decrypting with the shared key.
  
Authentication: 
    In the first step, Alice (client) initiates a connection request with Bob (server). Bob responds with his certificate. Alice accepts the certificate and authenticates it. Key Exchange: In this step, Alice sends the secret by encrypting it with Bob’s public key. Bob accepts the encrypted message and decrypts it with his own private key. Thus, keys are exchanged in this step. Data Exchange: In this step, data is shared between Alice and Bob. Alice sends data to Bob by encrypting it with the shared secret. Bob accepts it and decrypts it, and vice versa. Thus, data is shared between Alice and Bob.

3 certificates for Alice and Bob have been created with key sizes 1024, 2048 and 4096.
