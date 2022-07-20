# COSE CDDL

All [COSE](https://www.rfc-editor.org/authors/rfc9052.html) structures in a
single [CDDL](https://datatracker.ietf.org/doc/rfc8610/) [file](rfc9052.cddl).

The CDDL is extracted by the RFC document using these commands:

```sh
curl https://www.rfc-editor.org/authors/rfc9052.xml \
    | xmlstarlet sel -T -t -v '//sourcecode[@type="cddl"]' \
    > rfc9052.cddl
```

NOTE: the RFC is not officially published yet, though it's *very* unlikely to
change at this time.
