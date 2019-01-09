clone everything
checkout 4.0
symlink the dirs from Cura-package to $PACKAGE/debian
build with "dpkg-buildpackage -uc -s", install debs as you go
