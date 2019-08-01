# Helper scripts useful for Anonymizing Linux Distributions #

Library that can be used by other (anonymity related) packages that want to
programmatically get information about states of Tor. Common code, that is
often required. Includes bash and Python helper scripts.
## How to install `helper-scripts` using apt-get ##

1\. Download [Whonix's Signing Key]().

```
wget https://www.whonix.org/patrick.asc
```

Users can [check Whonix Signing Key](https://www.whonix.org/wiki/Whonix_Signing_Key) for better security.

2\. Add Whonix's signing key.

```
sudo apt-key --keyring /etc/apt/trusted.gpg.d/whonix.gpg add ~/patrick.asc
```

3\. Add Whonix's APT repository.

```
echo "deb https://deb.whonix.org buster main contrib non-free" | sudo tee /etc/apt/sources.list.d/whonix.list
```

4\. Update your package lists.

```
sudo apt-get update
```

5\. Install `helper-scripts`.

```
sudo apt-get install helper-scripts
```

## How to Build deb Package ##

Replace `apparmor-profile-torbrowser` with the actual name of this package with `helper-scripts` and see [instructions](https://www.whonix.org/wiki/Dev/Build_Documentation/apparmor-profile-torbrowser).

## Contact ##

* [Free Forum Support](https://forums.whonix.org)
* [Professional Support](https://www.whonix.org/wiki/Professional_Support)

## Donate ##

`helper-scripts` requires [donations](https://www.whonix.org/wiki/Donate) to stay alive!
