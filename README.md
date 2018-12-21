This is the repo to generate the [comparison site](https://kiwi0fruit.github.io/pystitch/).

# Building the Page

If you're modifying the markdown source, you'll need to install [knitty](https://github.com/kiwi0fruit/knitty) (only available on Github at the moment) together with all `dev` deps from [`setup.py`](https://github.com/kiwi0fruit/knitty/blob/master/setup.py). If you're just altering the CSS, you shouldn't need `knitty`.

To make the page, use:

```
make html
```

To call `knotr` on `src/usage.md` and re-generate html examples swap `Makefile` and `Makefile_old` names before running `make html` (this may require installing additional python packages). The included script will then walk through the markdown and HTML documents, weaving the two together.

To push the page to GitHub pages, use:

```
make github
```


## Install

On Windows you might need to install `make` first:

* Install [Msys2](http://www.msys2.org/)
* Run MSYS2 MinGW 64-bit
* Install make with `pacman -S make git base-devel`
* You may need to `source <...>/activate env` from Msys2 terminal before running `make`
