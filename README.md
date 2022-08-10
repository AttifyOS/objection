# Objection

Objection is a runtime mobile exploration toolkit, powered by Frida, built to help you assess the security posture of your mobile applications, without needing a jailbreak.

This is a snap package. Requires snapd. 

Snap is usually pre-installed on recent Ubuntu and derivatives. If not check https://snapcraft.io/docs/installing-snapd.

## Building from source

```
$ cd src
$ snapcraft --use-lxd
```

### Build Notes

To start a shell automatically on build error
```
$ snapcraft --use-lxd --debug
```

To get a shell after the priming stage
```
$ snapcraft prime --use-lxd --shell-after
```

To install the built snap
```
$ sudo snap install ./objection_1.11.0_amd64.snap --devmode
```

Start a shell in the snap environment
```
$  snap run --shell objection
```

To uninstall the snap
```
$  snap remove objection
```