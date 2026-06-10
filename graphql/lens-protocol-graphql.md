# Lens Protocol GraphQL API

The Lens API is a hosted GraphQL endpoint that indexes the Lens
Chain contracts and exposes queries and mutations for accounts,
posts (publications), feeds, follows, groups, apps, notifications,
and search. It is the primary read/write surface for most Lens
applications and is consumed by the Lens TypeScript SDK and React
SDK. Authentication uses Lens-issued bearer tokens obtained via a
wallet signature.

## Lens API (GraphQL)

**Endpoint:** https://api.lens.xyz/graphql

**Documentation:** https://lens.xyz/docs/api

**GraphQL Properties:**

- GraphQLEndpoint: https://api.lens.xyz/graphql

## Lens Authentication

Lens authentication uses a sign-in-with-Ethereum style challenge:
a client requests a signing message from the Lens API, the user
signs it with their wallet, and the API returns short-lived access
and refresh tokens scoped to a specific Account and App. The auth
flow supports owner, manager, and onboarding-user roles.

**Endpoint:** https://api.lens.xyz/graphql

**Documentation:** https://lens.xyz/docs/authentication

**References:**

- Documentation: https://lens.xyz/docs/authentication
