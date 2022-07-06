Cmenu – Calculator Menu
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

Cmenu is a simple shell script which allows you to calculate things.
This is useful if you want a quick solution to a math equation.

## Usage

Simply invoke the `` `# user` cmenu `` command and enter anything you
want. Use the `--copy` or `-c` argument if you want to copy the output.

``` sh
`# user` cmenu
`# user` cmenu -c clipboard # copy the output to clipboard
```

## Dependencies

1.  dmenu
2.  xclip (if you want to use the `copy` argument)

## Installation

### Universal

``` sh
`# user` git clone https://github.com/amarakon/cmenu
`# user` cd cmenu
`# root` make install
```

### Gentoo

``` sh
`# root` eselect repository add amarlay git https://github.com/amarakon/amarlay
`# root` emerge --sync amarlay
`# root` emerge x11-misc/cmenu
```

## Uninstallation

### Universal

``` sh
`# user` cd cmenu
`# root` make uninstall
```

### Gentoo

``` sh
`# root` emerge -c x11-misc/cmenu
# Remove my overlay (optional)
`# root` eselect-repository remove -f amarlay
`# root` emerge --sync
```
