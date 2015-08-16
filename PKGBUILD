# Maintainer: SpepS <dreamspepser at yahoo dot it>

_lv2=ssg
pkgname=lv2-ssg
pkgver=1.14
pkgrel=1
pkgdesc="Simple Sine Generator is the simplest LV2 synth plugin written in plain C, acting as template."
arch=(i686 x86_64)
url="http://nedko.arnaudov.name/soft/ssg/"
license=('GPL')
groups=('lv2-plugins')
depends=('lv2core')
source=("$url$_lv2-$pkgver.tar.bz2")
md5sums=('0b1ab43efafc3cf1761bfb77a27ad028')

build() {
  cd "$srcdir/$_lv2-$pkgver"

  make
}

package() {
  cd "$srcdir/$_lv2-$pkgver"

  # install lv2 plugin
  install -d "$pkgdir/usr/lib/lv2"
  cp -a $_lv2-1.lv2 "$pkgdir/usr/lib/lv2"
}

# vim:set ts=2 sw=2 et:
