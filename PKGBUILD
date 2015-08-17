# Maintainer: Tomasz Zok <tomasz.zok [at] gmail.com>
pkgname=nxclient3
pkgver=3.5.0
pkgrel=2
pkgdesc="NoMachine nxclient"
arch=('i686' 'x86_64')
url="https://www.nomachine.com/Select-Package-Linux&id=19"
license=('custom:nomachine')
provides=('nxclient')

if [ "${CARCH}" = "i686" ]; then
  source=(http://baobabmaster.unige.ch/download/linux/nxclient-${pkgver}-7.i386.tar.gz)
  md5sums=('0bc9f652cb294bc3eabc71e6ca6fe5dd')
else
  source=(http://baobabmaster.unige.ch/download/linux/nxclient-${pkgver}-7.x86_64.tar.gz)
  md5sums=('3d3ba27c7bf78f206964237892590140')
fi

package() {
  cd ${srcdir}
  install -d ${pkgdir}/usr/
  cp -a NX/ ${pkgdir}/usr/
}

# vim:set ts=2 sw=2 et:
