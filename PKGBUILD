
pkgname=libarchive
pkgver=3.0.4
pkgrel=1
pkgdesc="library that can create and read several streaming archive formats"
arch=('i386' 'x86_64')
url="http://libarchive.github.com/"
license=('BSD')
groups=('base')
depends=('zlib' 'bzip2')
options=(!libtool)
source=(https://github.com/downloads/libarchive/libarchive/libarchive-$pkgver.tar.gz)
md5sums=('af443ca9a10ddbcbf00f7ae34ca7fc16')

build() {
    cd $srcdir/$pkgname-$pkgver
    ./configure --prefix=/Library/ArchMac
    make
}

package() {
    cd $srcdir/$pkgname-$pkgver
    make DESTDIR=$pkgdir install
}
