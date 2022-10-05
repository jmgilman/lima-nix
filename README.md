# lima-nix

This repository contains a [Lima] template that will create a Ubuntu
VM with [nix] and [direnv] automatically installed and configured.

To use the template:

```text
limactl start --name=default https://raw.githubusercontent.com/jmgilman/lima-nix/master/nix.yml
```

This template is optimized for use with [nix-direnv]. In a folder with a properly
configured `.envrc` you should be able to run:

```text
lima
```

And you will (after a short time) be dropped into the appropriate development
shell. Alternatively, you can directly run commands with the `direnv` context
activated using the following:

```text
lima direnv exec . <cmd>
```

## Contributing

Check out the [issues] for items needing attention or submit your own and
then:

1. Fork the repo (<https://github.com/jmgilman/lima-nix/fork>)
2. Create your feature branch (git checkout -b feature/fooBar)
3. Commit your changes (git commit -am 'Add some fooBar')
4. Push to the branch (git push origin feature/fooBar)
5. Create a new Pull Request

[direnv]: https://direnv.net
[issues]: https://github.com/jmgilman/lima-nix/issues
[lima]: https://github.com/lima-vm/lima
[nix]: https://nixos.org
[nix-direnv]: https://github.com/nix-community/nix-direnv
