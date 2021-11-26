# Euro-Subdomains

Euro-Subdomains is a set of list of the most common subdomains for the most
popular TLDs. Currently, the supported TLDs are ".fr", ".de", ".ch", ".be",
".at", ".es", ".eu", ".it", ".lu", ".no", ".pt", ".se".

## Methodology

Cyberwatch fetch continuously the newly delivered TLS certificates from the log
servers from the [Certificate Transparency
Project](https://certificate.transparency.dev/). These certificates very often
contain valid domain names in the `cn` field or in the alternatives domain names
extension. These domain names are extracted from the certificates and stored in
a database.

For each supported TLD, the corresponding list represents the 1000 most frequent
subdomains for that TLD. Only the first labels of the domain names were used.

## Why ?

Enumeration of the subdomains of a domain is a common practice to discover it
resources associated with a domain name. These enumerations are often based on
dictionary or brute-force attacks, however, these dictionaries are not based on
the culture of the targets.

This project aims to provide an open dictionary with European common subdomains,
so that people can really discover assets more accurately.

## Licensing

This project is licensed under the [MIT
license](https://creativecommons.org/licenses/by/4.0/).
