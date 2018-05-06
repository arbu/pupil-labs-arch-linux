# Pupil Labs dependencies for Arch Linux
This repository provides some packages and fixes to run the [Pupil Labs Software](https://github.com/pupil-labs/pupil) on Arch Linux.

## Dependencies
Install the dependencies using `yaourt`:

```
yaourt -Pi libuvc-pupil-labs-git
yaourt -Pi python-pyre-git
yaourt -Pi python-pyav-pupil-labs-git
yaourt -Pi python-pyuvc-git
yaourt -Pi python-pyglui-git
yaourt -Pi python-pyndsi-git
yaourt -Pi pupil-labs-depends
```

or using `makepkg` (you need to install [python-ipaddress](https://aur.archlinux.org/packages/python-ipaddress/) and [ceres-solver](https://aur.archlinux.org/packages/ceres-solver/) manually):

```
(cd libuvc-pupil-labs-git && makepkg -si)
(cd python-pyre-git && makepkg -si)
(cd python-pyav-pupil-labs-git && makepkg -si)
(cd python-pyuvc-git && makepkg -si)
(cd python-pyglui-git && makepkg -si)
(cd python-pyndsi-git && makepkg -si)
(cd pupil-labs-depends && makepkg -si)
```

## Other
Apply `pupil-labs-arch-linux-fix-linker-settings.patch` to the Pupil Labs repository using `git apply`.
