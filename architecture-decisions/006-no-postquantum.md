## ADR 6: No Postquantum Primitives

### Context

With the coming of quantum computers (QC), the community have started discussing
about the use of quantum resistant algorithms in privacy enhancing technology.

### Decision

OTRv4 does not take advantage of quantum resistant algorithms for the following
reasons:

Firstly, OTRv4 aims to be possible and easy to implement in today's environments
in a reasonable time frame. OTRv4 only aims to lay the foundation for future
changes by adding version rollback protection, a DAKE, upgrades of primitives,
and non-interactive conversations.

Secondly, current quantum resistant algorithms and their respective libraries
are not ready for incorporation. Production level libraries may take up to 6-18
months to be ready. Future versions of the protocol may incorporate these
libraries and algorithms at that time.

### Consequences

OTRv4 does not use any algorithms which aim to provide effective resistance to
attacks done on quantum computers. If elliptic curve cryptography and 3072-bit
Diffie-Hellman can be attacked by quantum computers in the next upcoming years,
OTRv4's primitives will become unsafe and unusable. However, the use of a
3072-bit Diffie-Hellman "brace key" is used partly due to the potential of
quantum computers arriving earlier than predicted. We want extra protection
against post-conversation decryption of transcripts in this case.