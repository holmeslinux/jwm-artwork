# Maintainer: holmeslinux <holmes_holmes@live.com>

_snapshot=88b680538aeaa5d835860e1fb92d1ec890a19098
pkgname=jwm-artwork
pkgver=20160311
pkgrel=1
pkgdesc="artwork for jwm"
arch=('any')
license=('GPL3')
url="https://github.com/holmeslinux/$pkgname"
source=("$pkgname-$pkgver-$pkgrel.tar.gz::$url/archive/$_snapshot.tar.gz")
md5sums=('839be3199e87e34d98739130dbcd66ee')

package() {
#install buttons
	cd $srcdir/$pkgname-$_snapshot
	./configure --prefix=/usr/share/themes
	cp -r buttons $pkgdir/usr/share/themes
#install GrayOrange
	cd $srcdir/$pkgname-$_snapshot
	./configure --prefix=/usr/share/themes
	cp -r GrayOrange $pkgdir/usr/share/themes
}
