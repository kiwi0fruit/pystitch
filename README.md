This is the repo to generate the [comparison site](https://kiwi0fruit.github.io/pystitch/).

# Building the Page

If you're modifying the markdown source, you'll need to install
[stitch](https://github.com/kiwi0fruit/knitty) (only available on Github at the moment).
If you're just altering the CSS, you shouldn't need `stitch`.

To make the page, use

```
make html
```

This will call `stitch` on `src/usage.md`. The included script will then
walk through the markdown and HTML documents, weaving the two together.

## Install

On Windows you might need to install `make` first:

* Install [Msys2](http://www.msys2.org/)
* Run MSYS2 MinGW 64-bit
* Install make with `pacman -S make gettext base-devel`
* You may need to `source <...>/activate env` from Msys2 terminal before running `make`
