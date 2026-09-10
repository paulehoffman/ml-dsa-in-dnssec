This repo is an informal place to list implementations of DNSSEC (authoritative servers, validating resolvers, signers, ...) that support ML-DSA using codepoint 18 from [the IANA registry](https://www.iana.org/assignments/dns-sec-alg-numbers#dns-sec-alg-numbers-1) using the brief definition in [this draft](https://www.iana.org/go/draft-westerbaan-dnssec-mldsa-03).

Pull requests are welcome. This repo will probably become useless around March 2027 and may be frozen around then.

# Authoritative Servers

- [PowerDNS Auth](https://www.powerdns.com/). Supported on [master](https://github.com/PowerDNS/pdns/pull/17773), expected to be released for 5.2.0

# Validating Resolvers

- [Cloudflare 1.1.1.1](https://blog.cloudflare.com/post-quantum-dnssec-1111/)

- [PowerDNS Rec](https://www.powerdns.com/). Supported on [master](https://github.com/PowerDNS/pdns/pull/17773), expected to be released for 5.5.0

- [dnspython](https://github.com/rthalley/dnspython) (on master)

# Signers

- [dnspython](https://github.com/rthalley/dnspython) (on master)

# Test zones

- mldsa.huque.com (signed by Shumon Huque, alg 18, compact denial of existence)

- mldsan3.huque.com (signed by Shumon Huque, alg 18, pre-computed NSEC3)

- [dnstest.dev](https://dnstest.dev) by Cloudflare includes among others

  - `valid.mldsa44.dnstest.dev` signed only by 18
  - `dual-valid.mldsa44.dnstest.dev` signed by 13 and 18
  - `downgrade.mldsa44.dnstest.dev` is like dual, but alg 18 RRsigs are stripped to test downgrade protection of validator


# Libraries

https://codeberg.org/miekg/dns supports ML-DSA-44 since 0.6.98.

# Testing software

- https://codeberg.org/pawal/gonemaster supports ML-DSA-44 since 1.7.1.

- https://github.com/shuque/adns_server An authoritative DNS server for testing and prototyping

# Future
