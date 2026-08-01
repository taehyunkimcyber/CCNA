# ACLs

Access control list labs for filtering IPv4 traffic close to the correct
source or destination, verifying ACL hit counts, and troubleshooting common
direction and wildcard-mask mistakes.

## Labs

| # | Lab | Status |
|---:|---|---|
| 01 | [Static Standard and Extended ACLs](lab-01-static-standard-and-extended-acls/README.md) | Ready |
| 02 | [Extended ACLs for Services](lab-02-extended-acl-services/README.md) | Ready |

## Notes

- Standard ACLs match source IPv4 addresses only, so they are usually placed
  close to the destination.
- Extended ACLs match source, destination, and protocol/port details, so they
  are usually placed close to the source.
- Named extended ACLs can use sequence numbers, which makes it easier to
  insert, remove, and reorder specific permit or deny statements.
