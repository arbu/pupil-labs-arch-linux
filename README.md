# Pupil Labs dependencies for Arch Linux
This repository provides some packages and fixes to run the [Pupil Labs Software](https://github.com/pupil-labs/pupil) on Arch Linux.

## Dependencies
Install the remaining dependencies:

```
yaourt -Pi libuvc-pupil-labs-git
yaourt -Pi python-pyre-git
yaourt -Pi python-pyav-pupil-labs-git
yaourt -Pi python-pyuvc-git
yaourt -Pi python-pyglui-git
yaourt -Pi python-pyndsi-git
yaourt -Pi pupil-labs-depends
```

## Other
Apply `pupil-labs-arch-linux-fix-linker-settings.patch` to the Pupil Labs repository using `git apply`.
