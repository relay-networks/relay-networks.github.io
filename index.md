# Towards a Tectonic Traffic Shift? Investigating Apple's New Relay Network

Authors: TBA

## Abstract

Apple recently published its first Beta of the iCloud Private Relay, a privacy protection service with promises resembling the ones of VPNs. The architecture consists of two layers (ingress and egress), operated by disjoint providers. The service is directly integrated into Apple's operating systems and therefore provides a low entry level barrier for a large user base. It seems to be set up for major adoption with its relatively moderate entry-level price.

This paper analyzes the iCloud Private Relay from a network perspective and its effect on the Internet and future measurement-based research. We perform EDNS0 Client Subnet DNS queries to collect ingress relay addresses and find 1586 IPv4 addresses. Supplementary RIPE Atlas DNS measurements reveal 1575 IPv6 addresses. Knowledge about these addresses helps to passively detect clients communicating through the relay network. According to our scans, from January through April, ingress addresses grew by 20 %.

The analysis of our scans through the relay network verifies Apple’s claim of rotating egress addresses. Nevertheless, it reveals that ingress and egress relays can be located in the same autonomous system, thus sharing similar routes, potentially allowing traffic correlation.

## Ingress ECS Scan Data

Due to the data's size detailed ingress scan data is made available on an institution server when author anonymity is lifted.

- Ingress Scan Data: [all](https://github.com/relay-networks/relay-networks.github.io/tree/main/ingress-ecs-scan-data)
- QUIC (mask.icloud.com) Ingress Addresses:
    - [January](https://github.com/relay-networks/relay-networks.github.io/tree/main/ingress-ecs-scan-data/2022-01/ecs-scan-2022-01-14.ips)
    - [February](https://github.com/relay-networks/relay-networks.github.io/tree/main/ingress-ecs-scan-data/2022-02/ecs-scan-2022-02-05.ips)
    - [March](https://github.com/relay-networks/relay-networks.github.io/tree/main/ingress-ecs-scan-data/2022-03/ecs-scan-2022-03-25.ips)
    - [April](https://github.com/relay-networks/relay-networks.github.io/tree/main/ingress-ecs-scan-data/2022-04/ecs-scan-2022-04-22.ips)
    - additional data will be made available
- TCP (mask-h2.icloud.com) Ingress Addresses:
    - January: no data
    - [February](https://github.com/relay-networks/relay-networks.github.io/tree/main/ingress-ecs-scan-data/2022-02/ecs-scan-h2-2022-02-10.ips)
    - [March](https://github.com/relay-networks/relay-networks.github.io/tree/main/ingress-ecs-scan-data/2022-03/ecs-scan-h2-2022-03-25.ips)
    - [April](https://github.com/relay-networks/relay-networks.github.io/tree/main/ingress-ecs-scan-data/2022-04/ecs-scan-h2-2022-04-22.ips)
    - additional data will be made available

## Egress Archive

Egress IP ranges are available for selected days. For the future a daily archive starting in mid of May is available.

[Egress Archive](https://github.com/relay-networks/relay-networks.github.io/tree/main/egress-ip-ranges)

## iCloud Private Relay Scans

Scan data violates double blind requirements due to the location based egress selection of iCloud Private Relay. It will be made available when anonymity is lifted.
