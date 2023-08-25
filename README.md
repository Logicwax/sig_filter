Lets say you have a PGP clear signed message:

`echo -e "foo" | gpg --clearsign --armor --local-user user@foo.com`

and if it contains multiple signatures, you can filter out a specific keyID from the signatures with:
`sig_filter -f [keyId] < /path/to/sig.asc`

