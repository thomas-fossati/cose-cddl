# COSE CDDL

All [COSE](https://www.rfc-editor.org/rfc/rfc9052.html) structures in a
single [CDDL](https://datatracker.ietf.org/doc/rfc8610/) [file](rfc9052.cddl).

The CDDL is extracted from the RFC document using these commands:

```sh
curl https://www.rfc-editor.org/rfc/rfc9052.xml \
    | xmlstarlet sel -T -t -v '//sourcecode[@type="cddl"]' \
    > rfc9052.cddl
```
