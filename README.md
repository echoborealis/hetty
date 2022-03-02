<h1>
  <img src="https://hetty.xyz/img/hetty_light.svg#gh-light-mode-only" width="240"/>
  <img src="https://hetty.xyz/img/hetty_dark.svg#gh-dark-mode-only" width="240"/>
</h1>

[![Latest GitHub release](https://img.shields.io/github/v/release/dstotijn/hetty?color=25ae8f)](https://github.com/dstotijn/hetty/releases/latest)
[![Build Status](https://img.shields.io/endpoint.svg?url=https://actions-badge.atrox.dev/dstotijn/hetty/badge&label=build&logo=none&color=25ae8f)](https://github.com/dstotijn/hetty/actions/workflows/build-test.yml)
![GitHub download count](https://img.shields.io/github/downloads/dstotijn/hetty/total?color=25ae8f)
[![GitHub](https://img.shields.io/github/license/dstotijn/hetty?color=25ae8f)](https://github.com/dstotijn/hetty/blob/master/LICENSE)
[![Documentation](https://img.shields.io/badge/hetty-docs-25ae8f)](https://hetty.xyz/)

**Hetty** is an HTTP toolkit for security research. It aims to become an open
source alternative to commercial software like Burp Suite Pro, with powerful
features tailored to the needs of the infosec and bug bounty community.

<img src="https://hetty.xyz/img/hero.png" width="907" alt="Hetty proxy logs (screenshot)" />

## Features

- Machine-in-the-middle (MITM) HTTP proxy, with logs and advanced search
- HTTP client for manually creating/editing requests, and replay proxied requests
- Scope support, to help keep work organized
- Easy-to-use web based admin interface
- Project based database storage, to help keep work organized

👷‍♂️ Hetty is under active development. Check the <a
href="https://github.com/dstotijn/hetty/projects/1">backlog</a> for the current
status.

📣 Are you pen testing professionaly in a team? I would love to hear your
thoughts on tooling via [this 5 minute
survey](https://forms.gle/36jtgNc3TJ2imi5A8). Thank you!

## Getting started

💡 The [Getting started](https://hetty.xyz/docs/getting-started) doc has more
detailed install and usage instructions.

### Installation

The quickest way to install and update Hetty is via a package manager:

#### macOS

```sh
brew install hettysoft/tap/hetty
```

#### Linux

```sh
sudo snap install hetty
```

#### Windows

```sh
scoop bucket add hettysoft https://github.com/hettysoft/scoop.git
scoop install hettysoft/hetty
```

#### Other

Alternatively, you can [download the latest release from
GitHub](https://github.com/dstotijn/hetty/releases/latest) for your OS and
architecture, and move the binary to a directory in your `$PATH`. If your OS is
not available for one of the package managers or not listed in the GitHub
releases, you can compile from source _(link coming soon)_ or use a Docker image
_(link coming soon)_.

### Usage

Once installed, start Hetty via:

```sh
hetty
```

💡 Read the [Getting started](https://hetty.xyz/docs/getting-started) doc for
more details.

To list all available options, run: `hetty --help`:

```
$ hetty --help

Usage:
    hetty [flags] [subcommand] [flags]

Runs an HTTP server with (MITM) proxy, GraphQL service, and a web based admin interface.

Options:
    --cert         Path to root CA certificate. Creates file if it doesn't exist. (Default: "~/.hetty/hetty_cert.pem")
    --key          Path to root CA private key. Creates file if it doesn't exist. (Default: "~/.hetty/hetty_key.pem")
    --db           Database directory path. (Default: "~/.hetty/db")
    --addr         TCP address for HTTP server to listen on, in the form \"host:port\". (Default: ":8080")
    --chrome       Launch Chrome with proxy settings applied and certificate errors ignored. (Default: false)
    --verbose      Enable verbose logging.
    --json         Encode logs as JSON, instead of pretty/human readable output.
    --version, -v  Output version.
    --help, -h     Output this usage text.

Subcommands:
    - cert  Certificate management

Run `hetty <subcommand> --help` for subcommand specific usage instructions.

Visit https://hetty.xyz to learn more about Hetty.
```

## Documentation

📖 [Read the docs](https://hetty.xyz/docs)

## Support

Use [issues](https://github.com/dstotijn/hetty/issues) for bug reports and
feature requests, and
[discussions](https://github.com/dstotijn/hetty/discussions) for questions and
troubleshooting.

## Community

💬 [Join the Hetty Discord server](https://discord.gg/3HVsj5pTFP)

## Contributing

Want to contribute? Great! Please check the [Contribution
Guidelines](CONTRIBUTING.md) for details.

## Acknowledgements

- Thanks to the [Hacker101 community on Discord](https://www.hacker101.com/discord)
  for the encouragement and early feedback.
- The font used in the logo and admin interface is [JetBrains
  Mono](https://www.jetbrains.com/lp/mono/).

## Sponsors

<a href="https://www.tines.com/?utm_source=oss&utm_medium=sponsorship&utm_campaign=hetty">
<img src="https://hetty.xyz/img/tines-sponsorship-badge.png" width="140" alt="Sponsored by Tines">
</a>

## License

[MIT](LICENSE)

© 2022 Hetty Software
