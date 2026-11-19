# Studiny Writing Operator — Documentation

The Studiny Writing Operator is a private Vercel Integration for verifying deployment metadata during an owner-controlled Studiny Writing canary. Only the authorized Studiny owner may approve its installation. Install it on **`studiny-yaaelnet` only**.

## Vercel permissions

- **Projects — Read** for project identity and deployment settings.
- **Deployments — Read** for deployment status, identity, and assigned aliases.
- **Integration Configuration — Read** where required for the installation record.

Keep all other scopes disabled. Use short-lived access tokens only. The Integration's token provides metadata access. A separate one-shot operator handles any later canary opening under its own authorization and safeguards. Creating or installing the Integration leaves Studiny Writing activation unchanged. Learner-facing features operate independently of this Integration.

## Install, verify, and remove

1. In Vercel, keep visibility **Private**, select only the authorized project, and review the scopes before accepting. Complete the consent flow on the trusted operator computer.
2. Before use, the owner verifies the selected project, granted read scopes, credential expiry, and access to the expected project and deployment metadata. Stop if an unrelated project is accessible or a response exposes protected credentials.
3. When the operation is complete or access is withdrawn, uninstall the Integration in Vercel. Verify that the credential no longer authorizes access, and retire the corresponding operator credential and any temporary operator deployment.

[Terms of Use](TERMS.md) · [Privacy Policy](PRIVACY.md) · [Support](SUPPORT.md)
