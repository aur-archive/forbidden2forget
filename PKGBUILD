
# Maintainer: Dany Martineau <dany.luc.martineau gmail.com>

pkgname=forbidden2forget
pkgver=3.0.5
pkgrel=1
pkgdesc="Help french people to learn irregular verbs in english."
arch=('i686' 'x86_64')
url="http://congelli.kelio.org/prog_info_forbidden2forget.html"
license=('GPL')
depends=('wxgtk' 'desktop-file-utils')
madepends=('make' )
source=(http://fr.congelli.eu/download/forbidden2forget/forbidden2forget-3.0.5.tar.gz)
install=forbidden2forget.install
md5sums=('d530e61435db2777b2fb965e326519ca')

build() {
cd ${srcdir}/$pkgname-$pkgver
./configure --prefix=/usr
make
  }

package() {
cd ${srcdir}/$pkgname-$pkgver
make DESTDIR=${pkgdir} install
}
