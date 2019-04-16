Run `./clone-all` to clone everything

checkout 3.2-debian in Cura-packaging

apt install dpkg-dev

for PACKAGE in fdm_materials libCharon libSavitar libArcus Uranium CuraEngine cura-binary-data Cura; do
    checkout 3.2 (some repos don't have a 3.2 branch, use a tag instead of a newer branch if needed)
    ln -s ../Cura-package/${PACKAGE} debian
    dpkg-checkbuilddeps
    dpkg-buildpackage -uc -s
    install debs as you go
