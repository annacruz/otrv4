# Glossary of terms

* Backward secrecy
  - is when the compromise of a long-term key does not allow subsequent ciphertexts to be decripted by passive attackers. However future ciphertexts are vulnerable to active atackers.

* Conversation
  - is the exchange of messages between two sides, which can rely on an instant messaging mechanism able to send and receive said messages.

* Forward secrecy
  - is when the compromise of a long-term key does not allow ciphertexts encrypted with previous session keys to be decrypted.
  
* Initiator
  - is the party that will send the first material to start a DAKE transaction. In an interactive scenario is the party who answers to a request to start a conversation. In a non-interactive scenario is the party who publishes a set of pre-keys to a server.

* Secure channel
  - a channel is a way to transfer messages and is said to be secure if these messages can not be overheard or tampered with.

* Verify identity
  - the process where users verify that they are actually communicating with the parties they intend, in OTR this can be done verifing the party's fingerprint or using SMP