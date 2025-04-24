# Securden Provider

This guide will take you through the process of installing and using of Securden CLI to securely retrieve account credentials, keys, and secrets using APIs.

## Summary of Steps

1. Installation
2. Updating Securden CLI
3. Fetch credential via CLI commands

## 1. Installation

```hcl
scoop bucket add securden https://github.com/SecurdenDevOps/win-cli.git
```

```hcl
scoop install securden-cli
```

## 2. Updating Securden CLI

```hcl
scoop update securden-cli
```
## 3. Fetch credential via CLI commands

### Required

- `server_url` (String) Securden Server URL. Example: https://company.securden.com:5454.
- `authtoken` (String) Securden API Authentication Token.

### Securden Server URL

> **&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;You can get the ‘server_url’ from Securden by navigating to Admin >> General >> Securden Server Connectivity section in the Securden web interface.**

### API Token for Authentication

> **&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Securden server supports API token-based authentication for programmatic access to credentials. You can generate and copy the auth token from the Securden web interface by navigating to Admin >> API Access >> Create and Manage API Tokens.**

```hcl
securden-cli <command> --server-url <server-url> --authtoken <authtoken> <--params> 
```

---
-> If you have general questions or issues in using Securden Provider, you may raise a support request to devops-support@securden.com. Our support team will get back to you at the earliest and provide a timeline if there are issue fixes involved.