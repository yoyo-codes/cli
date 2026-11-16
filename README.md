# yoyo CLI

Deploy web demos to [Yoyo](https://yoyo.codes) from your terminal and get an
instant HTTPS URL.

This repository hosts the release builds of the `yoyo` CLI. Documentation
lives at [docs.yoyo.codes/cli/overview](https://docs.yoyo.codes/cli/overview/).

## Install

macOS or Linux:

```sh
curl -fsSL https://yoyo.codes/install.sh | sh
```

The script downloads the build for your OS and CPU, verifies its checksum, and
puts `yoyo` in `~/.local/bin`. Run it again to upgrade. Set `YOYO_INSTALL_DIR`
to install somewhere else, or `YOYO_VERSION` to pin a version.

Homebrew:

```sh
brew install yoyo-codes/tap/yoyo
```

[mise](https://mise.jdx.dev):

```sh
mise use -g github:yoyo-codes/cli
```

Windows: download the zip from the
[latest release](https://github.com/yoyo-codes/cli/releases/latest) and put
`yoyo.exe` on your `PATH`.

## Quick start

```sh
yoyo auth                     # paste an API token from Settings → API Tokens
yoyo deploy --name my-demo    # creates the project and deploys the folder
```

You're live at `https://my-demo-<username>.yoyo.codes`. After the first
deploy the folder is linked, so later deploys are just `yoyo deploy`.

## Support

Questions and bug reports: [support@yoyo.codes](mailto:support@yoyo.codes).
