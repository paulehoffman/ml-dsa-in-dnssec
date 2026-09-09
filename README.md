This repo is an informal place to list implementations of DNSSEC (authoritative servers, validating resolvers, signers, ...) that support ML-DSA using codepoint 18 from [the IANA registry](https://www.iana.org/assignments/dns-sec-alg-numbers#dns-sec-alg-numbers-1) using the brief definition in [this draft](https://www.iana.org/go/draft-westerbaan-dnssec-mldsa-03).

Pull requests are welcome. This repo will probably become useless around March 2027 and may be frozen around then.

# Authoritative Servers

# Validating Resolvers

# Signers

# Test zones

kochen-specker.info (signed by Bas Westerbaan)

mldsa.huque.com (signed by Shumon Huque)

# Libraries

https://codeberg.org/miekg/dns supports ML-DSA-44 since 0.6.98.

# Testing software

https://codeberg.org/pawal/gonemaster supports ML-DSA-44 since 1.7.1.

# Future

Peter van Dijk says "MLDSA44 will be in PowerDNS Recursor 5.5 and Auth 5.2."
See the [pull request](https://github.com/PowerDNS/pdns/pull/17773).

A [pull request](https://github.com/rthalley/dnspython/pull/1291) for the validator in dnspython.
