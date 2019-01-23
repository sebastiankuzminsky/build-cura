clone everything
checkout 4.0
symlink the dirs from Cura-package to $PACKAGE/debian
build with "dpkg-buildpackage -uc -s", install debs as you go

build order:
PACKAGES="fdm_materials libCharon libSavitar libArcus Uranium CuraEngine cura-binary-data Cura"
