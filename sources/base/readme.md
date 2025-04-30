# kimχ yocto demo

This repository aims to provide a quick way to grab yocto layers and
build a demo image for the [kimχ micro](https://labs.groupgets.com/kimchi-micro)

## Quick Start

Clone and update submodules

```
git clone https://github.com/groupgets/kimchi-yocto-demo.git
cd kimchi-yocto-demo
git submodule update --init
```

Create a build directory

```
MACHINE=kimchi DISTRO=fslc-wayland . ./setup-environment build-kimchi
```

Build an image

```
bitbake -k core-image-base
```

## Programming the Board

See the [kimχ micro documentation](https://labs.groupgets.com/kimchi-micro/software/programming.html) for a walkthrough on how to do this

## Reusing an existing build directory

If you've already run a build and want to enter the bitbake environment again, you can simply run:

```
. ./setup-environment build-kimchi
```

Important Note
============
GroupGets does not provide coding, firmware, or software support of any kind and will not respond to related requests. All software and firmware provided by GroupGets are offered solely as examples or potential starting points. These repositories may be outdated and are not guaranteed to function as intended.

We do not accept returns or offer replacements due to issues related to software, firmware, or code compatibility.

The software is provided "AS IS", without warranty of any kind, express or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose and non-infringement. In no event shall the authors or copyright holders be liable for any claim, damages, or other liability, whether in an action of contract, tort, or otherwise, arising from, out of, or in connection with the software or the use or other dealings in the software.
