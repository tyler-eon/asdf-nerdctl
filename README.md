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
- `newuidmap`/`newgidmap` (e.g. `sudo apt-get install -y uidmap`)

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

After the initial install, `containerd` should be running as a service and `nerdctl` should "just work". If it doesn't work then ensure the `containerd.service` is active and running (e.g. `systemctl --user status containerd.service`). If it is not active and running, try starting (or restarting) the service: e.g. `systemctl --user start containerd.service`.

If you want `containerd.service` to always be running, use `sudo loginctl enable-linger <user>` after starting `containerd.service`.

If `containerd.service` does not exist then installing the rootless containerd service failed silently for some reason. See this [Getting Started](https://rootlesscontaine.rs/getting-started/containerd/) guide for more information on how to ensure your system has the necessary dependencies installed and available.

Check [asdf](https://github.com/asdf-vm/asdf) readme for more instructions on how to install & manage versions.

# Contributing

Contributions of any kind welcome! See the [contributing guide](contributing.md).

[Thanks goes to these contributors](https://github.com/tyler-eon/asdf-nerdctl/graphs/contributors)!

# License

See [LICENSE](LICENSE) © [Tyler Eon](https://github.com/tyler-eon/)
