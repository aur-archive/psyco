# Maintainer: Douglas Soares de Andrade <dsa@aur.archlinux.org>
# Contributor: uggwar
# Contributor: William Rea <sillywilly@gmail.com>

pkgname=psyco
pkgver=1.6
pkgrel=4
pkgdesc="JIT compiler for Python"
arch=('i686')
url="http://psyco.sourceforge.net"
license=('MIT')
depends=('python' 'glibc')
source=(http://downloads.sourceforge.net/$pkgname/$pkgname-$pkgver-src.tar.gz)

build() {
    cd "$srcdir/psyco-$pkgver"
    python setup.py install --root="$pkgdir" --optimize=1
    install -D COPYING.txt "$pkgdir/usr/share/licenses/$pkgname/COPYING"
}
md5sums=('8816fca8ba521e05d18dde3e1a11b0bd')
