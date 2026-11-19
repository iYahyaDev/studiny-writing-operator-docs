# Studiny Writing Operator — Privacy Policy

This notice covers the private Studiny Writing Operator Vercel Integration. It is used by the authorized Studiny operator to verify that the expected project and deployment are in service during an internal canary operation.

## Data and purpose

The Integration may read Vercel project identifiers and configuration, deployment identifiers and status, source revision metadata, assigned domains and aliases, and its installation configuration where authorized. It uses this information to verify the selected project, deployment, and access scope. The workflow is designed to operate without reading or processing student essays or learner profiles.

The local OAuth flow handles a one-time authorization code, the Integration client credentials, and the installation identity. It also receives temporary tokens for authorized verification. The OAuth code and token values are used transiently by the local receiver. Validated Integration client credentials and installation details are stored in Windows Credential Manager for the authorized operator on the trusted Windows computer. Temporary tokens are limited to the approved read scopes and are checked against their reported expiry, with a maximum lifetime of one hour.

Local operational records may retain verification outcomes, timestamps, approved scope names, and token expiry. They are intended to exclude credential values, OAuth codes, and learner material. A temporary operator deployment may receive a short-lived metadata token for the approved operation. The reusable OAuth client secret stays on the operator computer.

## Revocation and retention

The owner can uninstall the Integration through Vercel to revoke installation access and remove its retained local credential. The owner can also retire the corresponding temporary operator deployment, if one was created. Vercel and any other applicable service providers handle their retained copies under their own policies. Removing active access does not imply immediate deletion of every retained copy.

For privacy or access questions, use the Studiny contact channel. [Support](SUPPORT.md) · [Vercel Privacy Notice](https://vercel.com/legal/privacy-policy)
