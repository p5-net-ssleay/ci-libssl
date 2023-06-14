# libssl tarballs for GitHub Actions

This repository hosts tarballs containing minimal reproducible builds of libssl
and libcrypto. They are designed to be used for testing
[Net-SSLeay](https://github.com/radiator-software/p5-net-ssleay) on
[GitHub Actions](https://github.com/features/actions) runners, and are not
guaranteed to be useful for any other purpose.

The libssl builds are distributed using
[GitHub releases](https://github.com/p5-net-ssleay/ci-libssl/releases): each
supported libssl version has its own release (and Git tag), which in turn
contains a tarball for each supported operating system as a release asset. Since
the tarballs are themselves built using GitHub Actions, only operating systems
[currently provided as virtual environments for GitHub-hosted runners](https://docs.github.com/en/free-pro-team@latest/actions/reference/specifications-for-github-hosted-runners#supported-runners-and-hardware-resources)
are supported.

Tarballs are currently built for the following libssl implementations:

* [LibreSSL](https://www.libressl.org) - stable releases in the following series
  only; development versions are omitted:
  * 2.0 series (2.0.5 - 2.0.6)
  * 2.1 series (2.1.5 - 2.1.10)
  * 2.2 series (2.2.2 - 2.2.9)
  * 2.3 series (2.3.3 - 2.3.10)
  * 2.4 series (2.4.2 - 2.4.5)
  * 2.5 series (2.5.3 - 2.5.5)
  * 2.6 series (2.6.3 - 2.6.5)
  * 2.7 series (2.7.2 - 2.7.5)
  * 2.8 series (2.8.2 - 2.8.3)
  * 2.9 series (2.9.2)
  * 3.0 series (3.0.2)
  * 3.1 series (3.1.1 - 3.1.5)
  * 3.2 series (3.2.2 - 3.2.7)
  * 3.3 series (3.3.3 - 3.3.6)
  * 3.4 series (3.4.1 - 3.4.3)
  * 3.5 series (3.5.2 - 3.5.4)
  * 3.6 series (3.6.1 - 3.6.2)
  * 3.7 series (3.7.2 - 3.7.3)
* [OpenSSL](https://www.openssl.org) - stable releases in the following branches
  only; alpha, beta, prerelease, and withdrawn versions are omitted:
  * 0.9.8 branch (0.9.8 - 0.9.8zh)
  * 1.0.0 branch (1.0.0 - 1.0.0t)
  * 1.0.1 branch (1.0.1 - 1.0.1u)
  * 1.0.2 branch (1.0.2 - 1.0.2u)
  * 1.1.0 branch (1.1.0 - 1.1.0l)
  * 1.1.1 branch (1.1.1 - 1.1.1q, 1.1.1s - 1.1.1t)
  * 3.0 branch (3.0.0 - 3.0.5, 3.0.7 - 3.0.9)
  * 3.1 branch (3.1.0 - 3.1.1)
