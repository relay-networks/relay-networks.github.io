# Towards a Tectonic Traffic Shift? Investigating Apple's New Relay Network

Accepted at IMC'22

Authors: Patrick Sattler, Juliane Aulbach, Johannes Zirngibl, Georg Carle

Preprint available [https://arxiv.org/abs/2207.02112](https://arxiv.org/abs/2207.02112)

Data archive for results used in this paper: [https://mediatum.ub.tum.de/1687050](https://mediatum.ub.tum.de/1687050)

## Abstract

Apple recently published its first Beta of the iCloud Private Relay, a privacy protection service with promises resembling the ones of VPNs. The architecture consists of two layers (ingress and egress), operated by disjoint providers. The service is directly integrated into Apple's operating systems and therefore provides a low entry level barrier for a large user base. It seems to be set up for major adoption with its relatively moderate entry-level price.

This paper analyzes the iCloud Private Relay from a network perspective and its effect on the Internet and future measurement-based research. We perform EDNS0 Client Subnet DNS queries to collect ingress relay addresses and find 1586 IPv4 addresses. Supplementary RIPE Atlas DNS measurements reveal 1575 IPv6 addresses. Knowledge about these addresses helps to passively detect clients communicating through the relay network. According to our scans, from January through April, ingress addresses grew by 20 %.

The analysis of our scans through the relay network verifies Apple’s claim of rotating egress addresses. Nevertheless, it reveals that ingress and egress relays can be located in the same autonomous system, thus sharing similar routes, potentially allowing traffic correlation.

## Ingress ECS Scan Data

- Ingress Scan Data: [all](https://github.com/relay-networks/relay-networks.github.io/tree/main/ingress-ecs-scan-data)
- QUIC (mask.icloud.com) Ingress Addresses:
    - [January](https://github.com/relay-networks/relay-networks.github.io/tree/main/ingress-ecs-scan-data/2022-01/ecs-scan-2022-01-14.ips) [(raw data)](https://github.com/relay-networks/relay-networks.github.io/tree/main/ingress-ecs-scan-data/2022-01/raw-results)
    - [February](https://github.com/relay-networks/relay-networks.github.io/tree/main/ingress-ecs-scan-data/2022-02/ecs-scan-2022-02-05.ips) [(raw data)](https://github.com/relay-networks/relay-networks.github.io/tree/main/ingress-ecs-scan-data/2022-02/raw-results)
    - [March](https://github.com/relay-networks/relay-networks.github.io/tree/main/ingress-ecs-scan-data/2022-03/ecs-scan-2022-03-25.ips) [(raw data)](https://github.com/relay-networks/relay-networks.github.io/tree/main/ingress-ecs-scan-data/2022-03/raw-results)
    - [April](https://github.com/relay-networks/relay-networks.github.io/tree/main/ingress-ecs-scan-data/2022-04/ecs-scan-2022-04-22.ips) [(raw data)](https://github.com/relay-networks/relay-networks.github.io/tree/main/ingress-ecs-scan-data/2022-04/raw-results)
    - weekly ingress IP addresses can be found in our [archive](https://github.com/relay-networks/relay-networks.github.io/tree/main/ingress-ecs-scan-data/archive)
- TCP (mask-h2.icloud.com) Ingress Addresses:
    - January: no data
    - [February](https://github.com/relay-networks/relay-networks.github.io/tree/main/ingress-ecs-scan-data/2022-02/ecs-scan-h2-2022-02-10.ips) [(raw data)](https://github.com/relay-networks/relay-networks.github.io/tree/main/ingress-ecs-scan-data/2022-02/raw-results-h2)
    - [March](https://github.com/relay-networks/relay-networks.github.io/tree/main/ingress-ecs-scan-data/2022-03/ecs-scan-h2-2022-03-25.ips) [(raw data)](https://github.com/relay-networks/relay-networks.github.io/tree/main/ingress-ecs-scan-data/2022-03/raw-results-h2)
    - [April](https://github.com/relay-networks/relay-networks.github.io/tree/main/ingress-ecs-scan-data/2022-04/ecs-scan-h2-2022-04-22.ips) [(raw data)](https://github.com/relay-networks/relay-networks.github.io/tree/main/ingress-ecs-scan-data/2022-04/raw-results-h2)
    - weekly ingress IP addresses can be found in our [archive](https://github.com/relay-networks/relay-networks.github.io/tree/main/ingress-ecs-scan-data/archive)

## Egress Archive

Egress IP ranges are available for selected days. A daily archive is available starting in mid of May is available.

- [Egress Archive](https://github.com/relay-networks/relay-networks.github.io/tree/main/egress-ip-ranges)
- [Daily Egress Archive](https://github.com/relay-networks/relay-networks.github.io/tree/main/egress-daily-archive)

## iCloud Private Relay Scans

Data now available: [Link](https://github.com/relay-networks/relay-networks.github.io/tree/main/igress-egress-scan)

## Cite
- [Bib](https://raw.githubusercontent.com/relay-networks/relay-networks.github.io/main/private-relay-22.bib)

```
@inproceedings{sattler2022tectonictrafficshift,
    author = {Sattler, Patrick and Aulbach, Juliane and Zirngibl, Johannes and Carle, Georg},
    title = {Towards a Tectonic Traffic Shift? Investigating Apple's New Relay Network},
    year = {2022},
    isbn = {9781450392594},
    publisher = {Association for Computing Machinery},
    address = {New York, NY, USA},
    url = {https://doi-org.eaccess.ub.tum.de/10.1145/3517745.3561426},
    doi = {10.1145/3517745.3561426},
    booktitle = {Proceedings of the 22nd ACM Internet Measurement Conference},
    pages = {449–457},
    numpages = {9},
    location = {Nice, France},
    series = {IMC '22}
}
```

## Contact

[Patrick Sattler](https://net.in.tum.de/~sattler): **sattler [AT] net.in.tum.de**
