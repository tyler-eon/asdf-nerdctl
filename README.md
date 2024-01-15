<div align="center">

# asdf-nerdctl [![Build](https://github.com/tyler-eon/asdf-nerdctl/actions/workflows/build.yml/badge.svg)](https://github.com/tyler-eon/asdf-nerdctl/actions/workflows/build.yml) [![Lint](https://github.com/tyler-eon/asdf-nerdctl/actions/workflows/lint.yml/badge.svg)](https://github.com/tyler-eon/asdf-nerdctl/actions/workflows/lint.yml)

[nerdctl](https://github.com/tyler-eon/nerdctl) plugin for the [asdf version manager](https://asdf-vm.com).

</div>

# Contents

- [Dependencies](#dependencies)
- [Install](#install)
- [Contributing](#contributing)
- [License](#license)

# Dependencies

- `bash`
- `curl`
- `tar`

# Install

Plugin:

```shell
asdf plugin add nerdctl
# or
asdf plugin add nerdctl https://github.com/tyler-eon/asdf-nerdctl.git
```

Once the plugin is added, find a version and install it.

```shell
# Show all installable versions
asdf list-all nerdctl

# Install specific version
asdf install nerdctl latest

# Set a version globally (on your ~/.tool-versions file)
asdf global nerdctl latest

# Now nerdctl commands are available
nerdctl version
```

After installing a new version, you need to run `containerd-rootless-setuptool.sh` to ensure your environment is set up appropriately. If you are having trouble with the installation or `nerdctl` is failing for some reason, try look at this [Getting Started](https://rootlesscontaine.rs/getting-started/containerd/) guide.

Check [asdf](https://github.com/asdf-vm/asdf) readme for more instructions on how to install & manage versions.

# Contributing

Contributions of any kind welcome! See the [contributing guide](contributing.md).

[Thanks goes to these contributors](https://github.com/tyler-eon/asdf-nerdctl/graphs/contributors)!

# License

See [LICENSE](LICENSE) © [Tyler Eon](https://github.com/tyler-eon/)
