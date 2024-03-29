# Dotfiles

When spinning up a new NixOS machine, you will need to copy over /etc/nixos/configuration.nix, and create an empty directory at ~/.config/home-manager/.

Then run
```bash
sudo nixos-rebuild switch
```

Now copy over everything in .config/home-manager, and run
```bash
home-manager switch
```

That should pretty much do it, although I haven't actually tested it so this is all still 'in theory'.

Oh and if you want to play with elixir, add the elixir_dev_flake.nix or the phoenix_dev_flake.nix to the root of your app and run
```bash
nix develop
```
