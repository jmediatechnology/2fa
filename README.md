scheb/2fa
=========

This bundle provides **[two-factor authentication](https://en.wikipedia.org/wiki/Multi-factor_authentication) for your
[Symfony](https://symfony.com/) application**.

[![Build Status](https://github.com/scheb/2fa/workflows/CI/badge.svg?branch=5.x)](https://github.com/scheb/2fa/actions?query=workflow%3ACI+branch%3A5.x)
[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/scheb/2fa/badges/quality-score.png?b=5.x)](https://scrutinizer-ci.com/g/scheb/2fa/?branch=5.x)
[![Code Coverage](https://scrutinizer-ci.com/g/scheb/2fa/badges/coverage.png?b=5.x)](https://scrutinizer-ci.com/g/scheb/2fa/?branch=5.x)
[![Latest Stable Version](https://poser.pugx.org/scheb/2fa/v/stable.svg)](https://packagist.org/packages/scheb/2fa)
[![Total Downloads](https://poser.pugx.org/scheb/2fa-bundle/downloads)](https://packagist.org/packages/scheb/2fa-bundle)
[![License](https://poser.pugx.org/scheb/2fa/license.svg)](https://packagist.org/packages/scheb/2fa)

<p align="center"><img alt="Logo" src="doc/2fa-logo.svg" /></p>

ℹ️ The repository contains bundle versions ≥ 5, versions 1-4 are located in [scheb/two-factor-bundle](https://github.com/scheb/two-factor-bundle).

---

The bundle is organized into sub-repositories, so you can choose the exact feature set you need and keep installed
dependencies to a minimum.

Core features provided by `scheb/2fa-bundle`:

- Interface for custom two-factor authentication methods
- Trusted IPs
- Multi-factor authentication (more than 2 steps)
- CSRF protection
- Whitelisted routes (accessible during two-factor authentication)

Additional features:

- Trusted devices (once passed, no more two-factor authentication on that device) (`scheb/2fa-trusted-device`)
- Single-use backup codes for when you don't have access to the second factor device (`scheb/2fa-backup-code`)
- QR codes to scan with your mobile device (`scheb/2fa-qr-code`)

Two-factor authentication methods:

- [TOTP authentication](https://en.wikipedia.org/wiki/Time-based_One-time_Password_algorithm) (`scheb/2fa-totp`)
- [Google Authenticator](https://en.wikipedia.org/wiki/Google_Authenticator)  (`scheb/2fa-google-authenticator`)
- Authentication code via email (`scheb/2fa-email`)

Installation
-------------
Follow the [installation instructions](doc/installation.md).

Documentation
-------------
Detailed documentation of all features can be found in the [doc](doc/index.md) directory.

Version Guidance
----------------

| Version        | Status                        | Symfony Version  |
|----------------|-------------------------------|------------------|
| [1.x][v1-repo] | EOL                           | >= 2.1, < 2.7    |
| [2.x][v2-repo] | EOL                           | ^2.6, ^3.0, ^4.0 |
| [3.x][v3-repo] | EOL                           | 3.4, ^4.0, ^5.0  |
| [4.x][v4-repo] | Security fixes until Nov 2021 | 3.4, ^4.0, ^5.0  |
| [5.x][v5-repo] | New features + Bug fixes      | 4.4, ^5.0        |

[v1-repo]: https://github.com/scheb/two-factor-bundle/tree/1.x
[v2-repo]: https://github.com/scheb/two-factor-bundle/tree/2.x
[v3-repo]: https://github.com/scheb/two-factor-bundle/tree/3.x
[v4-repo]: https://github.com/scheb/two-factor-bundle/tree/4.x
[v5-repo]: https://github.com/scheb/2fa/tree/5.x

Security
--------
For information about the security policy and know security issues, see [SECURITY.md](SECURITY.md).

Contributing
------------
Want to contribute to this project? See [CONTRIBUTING.md](CONTRIBUTING.md).

License
-------
This software is available under the [MIT license](LICENSE).
