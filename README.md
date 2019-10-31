Commands
--------

### Common commands

`pacman -Syu <pkg>`

Install (and update package list)

`pacman -S <pkg>`

Install only

`pacman -Rsc <pkg>`

Uninstall

`pacman -Ss <keywords>`

Search

`pacman -Syu`

Upgrade everything

### Query

`pacman -Qe`

List explictly-installed packages

`pacman -Ql <pkg>`

What files does this package have?

`pacman -Qii <pkg>`

List information on package

`pacman -Qo <file>`

Who owns this file?

`pacman -Qs <query>`

Search installed packages for keywords

### Orphans

`pacman -Qdt`

List unneeded packages

`pacman -Rns $(pacman -Qdtq)`

Uninstall unneeded packages

Avoid orphans by using `pacman -Rsc` to remove packages, which will remove unneeded dependencies.

### References

*   [Pacman tips and tricks](https://wiki.archlinux.org/index.php/Pacman/Tips_and_tricks) _(wiki.archlinux.org)_
