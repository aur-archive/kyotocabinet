# Maintainer: Alexander Duscheleit <jinks@archlinux.us>
# Contributor: Joaquim Pedro (osmano807) <osmano807@gmail.com>
pkgname=kyotocabinet
pkgver=1.2.76
pkgrel=1
pkgdesc="a modern implementation of DBM in C++"
arch=('i686' 'x86_64')
url="http://fallabs.com/kyotocabinet"
license=('LGPL3')
makedepends=('gcc>=3.1' 'make' 'pkgconfig' 'zlib')
depends=('zlib' 'gcc-libs')
source=("http://fallabs.com/${pkgname}/pkg/${pkgname}-${pkgver}.tar.gz")

build() {
  cd "$srcdir/$pkgname-$pkgver"

  ./configure --prefix=/usr
  make
}

package() {
  cd "$srcdir/$pkgname-$pkgver"

  make install DESTDIR="$pkgdir/"
}
sha512sums=('278db7b327eb4c21bf0137d9aa14fb67d74d5ce7ed1cb29fc9120d157a60de165ec0cf842903eb7952e8f998045ae585b958977fa973ba0e0773381de71d9f6a')
