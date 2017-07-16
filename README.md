#[NixOS](http://nixos.org) Pulse Demon [SLiM](http://slim.berlios.de/) Theme
![preview](https://github.com/robertodr/nixos-pulse-demon-slim/raw/master/preview.png)

The background image is the cover of the [Pulse
Demon](https://en.wikipedia.org/wiki/Pulse_Demon) album by
[Merzbow](https://en.wikipedia.org/wiki/Merzbow).
To use this theme in NixOS set your SLiM configuration settings like so:

```
services = {
  displayManager.slim = {
    enable = true;
    theme = pkgs.fetchurl {
      url = "https://github.com/robertodr/nixos-pulse-demon-slim/archive/v1.0.tar.gz";
      sha256 = "09z8y6fac9l9805f2j3q3zbidymx3s7hysx23vb07pc1s4n6874x";
    };
  }; 
};
```
