# Security Policy

## Reporting Security Issues

Please email security@flipthiscrypto.com for any security vulnerabilities instead of using GitHub issues.

## What's Secure Here

- ✅ No hardcoded secrets, API keys, or credentials
- ✅ No sensitive environment variables committed
- ✅ .gitignore properly configured
- ✅ Dependencies kept up to date
- ✅ External API calls use environment variables only

## Contributing Securely

1. Never commit `.env`, `.key`, credentials, or token files
2. Use `.env.example` to document required environment variables
3. Keep dependencies updated (`npm audit`, `pip audit`, etc.)
4. Report security issues confidentially
5. Don't log sensitive data (API keys, tokens, passwords, PII)

## Production Deployment

Before deploying:
- [ ] All secrets are in environment variables
- [ ] No `.env` files are committed
- [ ] Dependencies are audited and updated
- [ ] Sensitive logs are disabled
- [ ] HTTPS is enforced

---

Last Updated: 2026-02-26
