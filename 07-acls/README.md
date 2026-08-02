# ACLs

Access control list labs for filtering IPv4 traffic close to the correct
source or destination, verifying ACL hit counts, and troubleshooting common
direction and wildcard-mask mistakes.

Status: complete.

## Labs

| # | Lab | Status | Packet Tracer file |
|---:|---|---|---|
| 01 | [Static Standard and Extended ACLs](lab-01-static-standard-and-extended-acls/README.md) | Complete | `lab-01-static-standard-and-extended-acls/packet-tracer/01-static-acl.pkt` |
| 02 | [Extended ACLs for Services](lab-02-extended-acl-services/README.md) | Complete | `lab-02-extended-acl-services/packet-tracer/lab-02-extended-acl-services.pkt` |

## Notes

- Standard ACLs match source IPv4 addresses only, so they are usually placed
  close to the destination.
- Extended ACLs match source, destination, and protocol/port details, so they
  are usually placed close to the source.
- Named extended ACLs can use sequence numbers, which makes it easier to
  insert, remove, and reorder specific permit or deny statements.
