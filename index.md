## IPv6

- continuing the IPv6 target generation work
  - [entropy/ip](https://dl.acm.org/citation.cfm?id=2987445)
  - [IPv6 target generation](https://conferences.sigcomm.org/imc/2017/papers/imc17-final245.pdf)

- IPv6 header comparison
  - triggered by another IPv4-only paper
  - record route doesn't really exist; what have people written drafts for or prototyped?
  - critically: what actually passes? Does the routing header actually pass through? Can it be used?
  - related header extension work [at TMA2017](http://tma.ifip.org/wp-content/uploads/sites/7/2017/06/tma2017_paper22.pdf)
  - discussed briefly with authors of [this IMC2017 paper](https://conferences.sigcomm.org/imc/2017/papers/imc17-final174.pdf)

- open firewall policies: what actually passes through?
  - can, say, Atlas probes send unsolicited pings to each other (ICMP/UDP/TCP?)? Addressing may be global, but what firewalling exists, and where?
  - related: the PMTUD problem

- the KSK rollover
  - [ripe74 preso with original timeline, slide 25](ripe74.ripe.net/wp-content/uploads/presentations/25-RIPE74-lewis-submission.pdf)
  - when bumping up over 1280 bytes, do we trigger PMTUD glitches, and can we use the k-root to pinpoint them?

- IPv6 diffs
  - diff between originating ASNs in BGP dumps
  - diff in AS hops between pairs of hosts
  - diff in AS paths between pairs of hosts: peering distinctions
  - 

- IPv6 and anycast stability
  - Wei and Heidemann: [anycast to DNS roots on v4](http://tma.ifip.org/wp-content/uploads/sites/7/2017/06/tma2017_paper39.pdf)
  - but the v6 question is left unanswered, and it'd be really interesting
  - I imagine it's the same in most cases, but peering will differ and that may affect behaviour (for better or worse)

- Spoofing:
  - [this paper](https://conferences.sigcomm.org/imc/2017/papers/imc17-final24.pdf) is great but doesn't touch on the v6 data

- Threats in the IPv6 world
  - botnet traffic, amplification attacks, continuous sweeping: all commonplace in IPv4
  - the IPv6 space modifies how people attack it or measure it
  - so, what does this traffic look like in the IPv6 side? does it exist at all?

- v6 growth using atlas probes
  - [https://sdstrowes.co.uk/misc/atlas/index.html](https://sdstrowes.co.uk/misc/atlas/index.html)

- survey scanning techniques
  - go right back to the early stuff
  - see also [Characterizing the IPv6 Security Landscape by Large-Scale Measurements](https://link.springer.com/chapter/10.1007%2F978-3-319-20034-7_16) (2015)

## IPv4

- better studies of IPv4 transfer markets
  - [https://labs.ripe.net/Members/wilhelm/ipv4-transfers-in-the-ripe-ncc-service-region](IPv4 Transfers in the RIPE NCC Service Region)
  - [https://www.ripe.net/manage-ips-and-asns/resource-transfers-and-mergers/transfer-statistics](IPv4 Transfer Statistics)

## Archaeology

- Things get deprecated in standards. But what still works?
- conventional wisdom was that IPv4 Record Route was useless, but a paper in 2017 refutes that: [https://conferences.sigcomm.org/imc/2017/papers/imc17-final174.pdf](the Record Route Option is an Option)
- So what else works?
  - [rfc1393](https://tools.ietf.org/html/rfc1393)?
  - [IPv6 Routing Headers](https://www.iana.org/assignments/ipv6-parameters/ipv6-parameters.xhtml#ipv6-parameters-3)?

