# autopac

Automatically download package updates for Arch Linux.

## Installing

```bash
$ makepkg -si
==> Making package: autopac 1.0.0-1 ...
```

## Usage

The package automatically enables the `autopac` systemd timer. It checks for updates once per day at a random time.
