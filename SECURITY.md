# Security policy

## Supported versions

Security fixes target the latest release and the current `main` branch. Older versions may not receive fixes.

## Report a vulnerability

Please do not disclose an exploitable issue in a public issue or pull request. Use GitHub's **Report a vulnerability** option on the repository's **Security** tab if it is available. If it is not available, contact the maintainer privately through their GitHub profile to arrange a private report.

Include the affected version or commit, reproduction steps, expected and actual behavior, and the possible impact. Please redact player data, webhook URLs, tokens, and other secrets. Allow time for investigation and a fix before public disclosure.

For ordinary bugs that do not expose a security issue, use a GitHub issue.

## Deployment guidance

Keep permission checks, purchase fulfillment, and trusted game state on the server. Treat all client remote arguments as untrusted, even when using `RemoteGuard` or `RateLimiter`. Store webhook URLs in Roblox secrets, never in replicated modules or committed files. Rotate any secret that has been exposed.
