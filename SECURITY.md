# Security Policy

## Reporting A Security Issue

If you discover a security issue, please open a GitHub issue with a clear description and mark it as security-related. Do not include active credentials, private tokens, cookies, private user data, or exploitable secrets in the issue body.

If the issue involves sensitive information, first describe the type of risk without publishing the secret itself.

## What Not To Commit

Never commit:

- API keys
- Tokens
- Cookies
- Passwords
- Private account data
- Private user data
- Private messages
- Internal evidence records
- Unlicensed media assets
- Voice samples or likeness data without authorization

## If A Secret Is Accidentally Exposed

If a credential or private file is exposed:

1. Stop using the exposed credential immediately.
2. Revoke or rotate the credential at the provider.
3. Remove the file from the repository.
4. Review Git history and decide whether history rewriting is necessary.
5. Document the incident and the remediation steps.

## Supported Scope

This project is primarily workflow documentation and agent instructions. Security review focuses on avoiding credential leaks, private data exposure, unauthorized asset publication, unsafe platform access patterns, and misleading automation claims.
