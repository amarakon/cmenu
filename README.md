Rmenu – R Menu
================

## Contents

-   [Usage](#usage)
-   [Dependencies](#dependencies)
-   [Installation](#installation)
    -   [Universal](#universal)
    -   [Gentoo](#gentoo)
-   [Uninstallation](#uninstallation)
    -   [Universal](#universal-1)
    -   [Gentoo](#gentoo-1)

Rmenu is a simple shell script which allows you to run R expressions in
Dmenu. This is useful if you want a quick solution to a math equation.
Or if you just want to run a general R expression.

## Usage

Simply invoke the `rmenu` command and enter anything you want. Use the
`--copy` or `-c` argument if you want to copy the output to your
clipboard.

``` sh
`# user` rmenu
`# user` rmenu -c # copy output to clipboard
```

## Dependencies

1.  Dmenu
2.  Xclip (if you want to use the `copy` argument)

## Installation

### Universal

``` sh
`# user` git clone https://github.com/amarakon/rmenu
`# user` cd rmenu
`# root` make install
```

### Gentoo

``` sh
`# root` eselect repository add amarlay git https://github.com/amarakon/amarlay
`# root` emerge --sync amarlay
`# root` emerge x11-misc/rmenu
```

## Uninstallation

### Universal

``` sh
`# user` cd rmenu
`# root` make uninstall
```

### Gentoo

``` sh
`# root` emerge -c x11-misc/rmenu
# Remove my overlay (optional)
`# root`
```