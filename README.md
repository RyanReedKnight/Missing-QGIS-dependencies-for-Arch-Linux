# Missing QGIS dependncies

It apears that qgis in the Arch Linux repos does not automatically include all of the neccesary dependencies
for the application to run as expected, as when I initialy installed it, various errors related to missing
python modules came up.

When I installed these dependencies, qgis, installed via pacman, ran without these initial errors.
I found most of the packages by digging through the comments in [this bug report](https://bugs.archlinux.org/task/77947?project=1&string=qgis), I do not
know if they are all necessary.

For those who dont know, run the following command in a directory with the txt file to install all of the packages.
```
sudo pacman -Syu --needed --noconfirm - < missing-qgis-packages.txt
```

If you try it and errors persist, I would appreciate you letting me know.
