# NAT and PAT

Network Address Translation labs for static NAT, dynamic NAT pools, PAT
overload, inside/outside interface selection, translation-table verification,
and common NAT troubleshooting mistakes.

Status: complete.

## Labs

| # | Lab | Status | Packet Tracer file |
|---:|---|---|---|
| 01 | [Static NAT and PAT](lab-01-static-nat-and-pat/README.md) | Complete | `lab-01-static-nat-and-pat/packet-tracer/lab-01-static-nat-and-pat.pkt` |
| 02 | [Dynamic NAT and PAT](lab-02-dynamic-nat-and-pat/README.md) | Complete | `lab-02-dynamic-nat-and-pat/packet-tracer/lab-02-dynamic-nat-and-pat.pkt` |

## Notes

- Static NAT creates a fixed one-to-one mapping between an inside local address
  and an inside global address.
- Dynamic NAT creates temporary one-to-one mappings from a configured address
  pool.
- PAT overload lets many inside hosts share one public IPv4 address by tracking
  Layer 4 port numbers.
- NAT is configured on the edge router, with `ip nat inside` on trusted LAN
  interfaces and `ip nat outside` on the ISP-facing interface.
- NAT does not replace routing. The outside router still needs a route back to
  any inside global address that is not directly connected.
