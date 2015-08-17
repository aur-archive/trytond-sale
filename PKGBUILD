# Maintainer: Robin Baumgartner <robin@baumgartners.ch>
pkgname=trytond-sale
_pkgname=trytond_sale
pkgver=3.4.1
_pkgdir=3.4
pkgrel=1
pkgdesc="The sale module of the Tryton application platform"
arch=('any')
url='http://www.tryton.org/'
license=('GPL3')
groups=('trytond-modules')
depends=('trytond>=3.4' 'trytond-account>=3.4' 'trytond-account-invoice>=3.4' 'trytond-account-invoice-stock>=3.4' 'trytond-account-product>=3.4' 'trytond-company>=3.4' 'trytond-currency>=3.4' 'trytond-party>=3.4' 'trytond-product>=3.4' 'trytond-stock>=3.4')
makedepends=('python2-distribute')
source=("http://downloads.tryton.org/$_pkgdir/$_pkgname-$pkgver.tar.gz")
md5sums=("6d39674202954732709154359dcbbe85")

build() {
  cd $srcdir/$_pkgname-$pkgver
  python2 setup.py build
}

package() {
  cd $srcdir/$_pkgname-$pkgver
  python2 setup.py install --root=$pkgdir
}