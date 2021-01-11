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

* [OpenSSL](https://www.openssl.org) 0.9.8 branch (0.9.8 - 0.9.8zh)
