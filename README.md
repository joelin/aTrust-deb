# build

mkdir -p extract/DEBIAN

mkdir build

dpkg-deb -x aTrustInstaller_amd64.deb extract

dpkg-deb -e aTrustInstaller_amd64.deb extract/DEBIAN

dpkg-deb -b extract build/