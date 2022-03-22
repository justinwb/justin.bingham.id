---
layout: default
---

## Decentralization

I've spent several years focusing on decentralized Web3 patterns and protocols. 
The diversity of protocols and communities can be staggering, but the problems
and issues are remarkably consistent.

I've been most attracted to discovering common patterns that can
solve broad decentralization problems, and can in turn be applied and
implemented by distinct protocols for better interoperability.

### Identity and Authentication

Most single-sign-on experiences today are siloed to a given organization or
service. Ideally we could "sign-in once" across all applications and services that 
we engage with, and do so without having to rely on a centralized 
service like Google or Facebook (e.g. Login with Google, Login with Facebook).

The combination of decentralized identifiers like [DIDs](https://www.w3.org/TR/did-core/)
and compatible authentication protocols make this possible, but this area is
emerging and in flux.

I've contributed to the [Solid-OIDC Protocol](https://solid.github.io/solid-oidc/), 
which extends the widely adopted [OAuth2](https://www.rfc-editor.org/rfc/rfc6749) and 
[OpenID Connect](https://openid.net/specs/openid-connect-core-1_0.html) standards
for decentralized use cases, plugging well-known security issues (e.g. token replay)
that are commonplace in decentralized scenarios via 
[Demonstration of Proof of Possession (DPoP)](https://datatracker.ietf.org/doc/html/draft-ietf-oauth-dpop). 
I developed a [Solid-OIDC Java Library](https://github.com/janeirodigital/sai-java) for client authentication, and
have contributed to efforts to add decentralized authentication (DPoP, DID, etc.) 
to [Keycloak](https://keycloak.org).

### Decentralized Data Storage

Decentralized data storage is an essential complement to distributed ledgers and
the decentralized ecosystem as a whole. Much of my time has been devoted to
the evolution of open-standards for decentralized data.

I'm a contributing author of the [Solid Protocol](https://solidproject.org/TR/protocol),
invented by [Sir Tim Berners-Lee]([Sir Tim Berners-Lee](https://www.w3.org/People/Berners-Lee/)) 
at MIT, which uses the existing infrastructure of the 
Web as a medium for decentralized data. I've spent considerable time applying
[application](#application-interoperability) and [data interoperability](#data-interoperability) 
patterns across data protocols like Solid and [IPFS](https://ipfs.io).

### Data Interoperability

In a robust, decentralized ecosystem, disparate applications should be able
to interoperate over the same data. Specifically:

1. Applications have to be able to read and write the same data without breaking it
2. Applications must be able to discover and navigate complex data structures.
3. Individual components of complex data structures must be modular and interchangeable

I co-authored the [Shape Trees Specification](https://shapetrees.org/TR/specification),
which provides self-identifying data structures that disparate machines can interpret, 
validate, read, and write without breaking compatibility with other applications.
They pack resources into "little virtual trees" that provide machine to machine 
interoperability. These packages of data are easy for humans to understand, 
because they can be composed into familiar objects like medical records, notes, 
notebooks, calendars, and financial records. 

I developed the 
[shapetrees-java](https://github.com/janeirodigital/shapetrees-java)
library which allows servers or clients to parse and apply shape tree validation
against collections of resources.

### Application Interoperability

Applications need to be able to express what type of data
they want access to, and controllers must be able to securely decide whether
they want to give them access to that data. This has to work for all kinds of
data, and it needs to be <b>easy to understand</b>.

I co-authored the 
[Application Interoperability Specification](https://solid.github.io/data-interoperability-panel/specification/)
which details how data controllers can authorize disparate applications and
services to access subsets of their data in decentralized personal data stores.

I developed the
[sai-java](https://github.com/janeirodigital/sai-java)
library which allows for the rapid creation of fully-interoperable, consent-aware,
decentralized applications in the Solid ecosystem.

### Verifiable Credentials

Working in close [collaboration with RSA Labs](https://www.janeirodigital.com/blog/new-partnership-brings-enterprise-security-to-the-decentralized-web/),
we've applied [Verifiable Credentials](https://www.w3.org/TR/vc-data-model/) to
solve real-world problems in the decentralized ecosystem, and helped to establish
[RSA Mercury](https://mercury.rsalabs.com/), a suite of cloud-hosted services
to enable companies to easily use verifiable credentials.

