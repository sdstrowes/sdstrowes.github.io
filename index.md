## IPv6

- continuing the IPv6 target generation work
  - [entropy/ip](https://dl.acm.org/citation.cfm?id=2987445)
  - [IPv6 target generation](https://conferences.sigcomm.org/imc/2017/papers/imc17-final245.pdf)

- IPv6 header comparison
  - triggered by another IPv4-only paper
  - record route doesn't really exist; what have people written drafts for or prototyped?
  - critically: what actually passes? Does the routing header actually pass through? Can it be used?
  - related header extension work (at TMA2017)[http://tma.ifip.org/wp-content/uploads/sites/7/2017/06/tma2017_paper22.pdf]
  - discussed briefly with authors of (this IMC2017 paper)[https://conferences.sigcomm.org/imc/2017/papers/imc17-final174.pdf]

- open firewall policies: what actually passes through?
  - can, say, Atlas probes send unsolicited pings to each other (ICMP/UDP/TCP?)? Addressing may be global, but what firewalling exists, and where?
  - related: the PMTUD problem

- IPv6 diffs
  - diff between originating ASNs in BGP dumps
  - diff in AS hops between pairs of hosts
  - diff in AS paths between pairs of hosts: peering distinctions
  - 

- IPv6 and anycast stability
  - Wei and Heidemann: (anycast to DNS roots on v4)[http://tma.ifip.org/wp-content/uploads/sites/7/2017/06/tma2017_paper39.pdf]
  - but the v6 question is left unanswered, and it'd be really interesting
  - I imagine it's the same in most cases, but peering will differ and that may affect behaviour (for better or worse)

- Spoofing:
  - (this paper)[https://conferences.sigcomm.org/imc/2017/papers/imc17-final24.pdf] is great but doesn't touch on the v6 data

- v6 growth using atlas probes
  - (https://sdstrowes.co.uk/misc/atlas/index.html)[https://sdstrowes.co.uk/misc/atlas/index.html]

- survey scanning techniques
  - go right back to the early stuff

