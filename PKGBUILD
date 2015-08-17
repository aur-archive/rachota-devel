# Maintainer: Baobab <megavillain at gmail dot com>

pkgname=rachota-devel
pkgver=2.4.131031
_pkgver=${pkgver:0:3}
pkgrel=1
pkgdesc="A portable timetracker for personal projects (development version)"
arch=('any')
url="http://rachota.sourceforge.net/"
license=('CDDL')
depends=('java-runtime')
provides=(rachota)
conflicts=(rachota)
source=("http://downloads.sourceforge.net/rachota/rachota_${_pkgver/.}.jar"
        "rachota.desktop"
        "rachota.sh")
md5sums=('e065a1e0805e72adca26fcbd4c0fe0b8'
         '8f10dc0dc9f6f71838b5109c24bf9c6b'
         'bcbf041aa83d064a1d753da5b8439c29') 

build() {
  cd "$srcdir"
  install -Dm644 rachota_${_pkgver/.}.jar "$pkgdir/usr/share/java/rachota/rachota.jar"
  install -Dm755 rachota.sh "$pkgdir/usr/bin/rachota"
  install -Dm644 org/cesilko/rachota/gui/images/logo_48.png "$pkgdir/usr/share/pixmaps/rachota.png"
  install -Dm644 rachota.desktop "$pkgdir/usr/share/applications/rachota.desktop"
}
