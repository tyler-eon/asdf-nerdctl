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

**TODO: adapt this section**

- `bash`, `curl`, `tar`, and [POSIX utilities](https://pubs.opengroup.org/onlinepubs/9699919799/idx/utilities.html).
- `SOME_ENV_VAR`: set this environment variable in your shell config to load the correct version of tool x.

# Install

Plugin:

```shell
asdf plugin add nerdctl
# or
asdf plugin add nerdctl https://github.com/tyler-eon/asdf-nerdctl.git
```

nerdctl:

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

Check [asdf](https://github.com/asdf-vm/asdf) readme for more instructions on how to
install & manage versions.

# Contributing

Contributions of any kind welcome! See the [contributing guide](contributing.md).

[Thanks goes to these contributors](https://github.com/tyler-eon/asdf-nerdctl/graphs/contributors)!

# License

See [LICENSE](LICENSE) © [Tyler Eon](https://github.com/tyler-eon/)
