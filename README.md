# Securden Command Line Interface - Windows

This guide will take you through the process of installing and getting data through Securden CLI using pre-defined commands. 

## Summary of Steps

1. Installation
2. Updating Securden CLI
3. Fetch credential via CLI commands

## Prerequisites 

1. Scoop Package Manager

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

```hcl
securden-cli <command> --server-url <server-url> --authtoken <authtoken> <--params> 
```

---
-> If you have general questions or issues in using Securden Command Line Interface, you may raise a support request to devops-support@securden.com. Our support team will get back to you at the earliest and provide a timeline if there are issue fixes involved.