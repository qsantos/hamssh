# HamSSH

Encryption-less Variant of OpenSSH for amateur radio

International bodies and local governments grants special rights to operators of the [amateur radio service](https://en.wikipedia.org/wiki/Amateur_radio).
This allows free tinkering and experimentation with wireless technology.
In exchange, all communications should be performed [in the clear](https://qsantos.fr/2022/12/21/ham-crypto/).

However, this does not preclude the use of cryptography altogether.
This project allows using SSH over in the amateur radio service, such as [AMPRNet](https://en.wikipedia.org/wiki/AMPRNet).
This can be useful for secure authentication without passwords.

**Note:** all communications are unencrypted, **do not use passwords** in a HamSSH session

See also [HamFox](https://github.com/qsantos/hamfox).

# Installation

This project uses the same build process as the OpenSSH project on which it is built upon.
All installation names have been prefixed with “ham”, so there should be no conflict with regular OpenSSH.

```
autoreconf
./configure
make -j$(nproc)
sudo make install
```

You can also look at the [original README](README.md.orig).
