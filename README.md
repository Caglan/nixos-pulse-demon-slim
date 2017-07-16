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
    defaultUser = "roberto";
    theme = pkgs.fetchurl {
      url = "https://github.com/edwtjo/nixos-pulse-demon-slim/archive/v1.0.tar.gz";
      sha256 = "13bm7k3p6k7yq47nba08bn48cfv536k4ipnwwp1q1l2ydlp85r9d";
    };
    extraConfig = ''
      hidecursor false
    '';
  }; 
};
```
