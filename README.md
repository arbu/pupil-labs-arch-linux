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
yaourt -Pi ceres-solver-shared
yaourt -Pi pupil-labs-depends
```

or using `makepkg`:

```
(git clone https://aur.archlinux.org/python-ipaddress.git && cd python-ipaddress && makepkg -si)
(cd libuvc-pupil-labs-git && makepkg -si)
(cd python-pyre-git && makepkg -si)
(cd python-pyav-pupil-labs-git && makepkg -si)
(cd python-pyuvc-git && makepkg -si)
(cd python-pyglui-git && makepkg -si)
(cd python-pyndsi-git && makepkg -si)
(cd ceres-solver-shared && makepkg -si)
(cd pupil-labs-depends && makepkg -si)
```

## Other
Apply `pupil-labs-fix-python_boost-dependency.patch` to the Pupil Labs repository using `git apply`.
