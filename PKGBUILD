# Maintainer: holmeslinux <holmes_holmes@live.com>

pkgname=jwm-artwork
pkgver=20160311
pkgrel=1
pkgdesc="artwork for jwm"
arch=('any')
license=('GPL3')
url="https://github.com/holmeslinux/$pkgname"
_snapshot=88b680538aeaa5d835860e1fb92d1ec890a19098
source=("$pkgname-$pkgver-$pkgrel.tar.gz::$url/archive/$_snapshot.tar.gz")
md5sums=('839be3199e87e34d98739130dbcd66ee')

prepare() {
	# fix file permissions
	chmod -x $srcdir/$pkgname-$_snapshot/buttons/jwm/*
}

package() {
	cd $srcdir/$pkgname-$_snapshot
	install -dm755 $pkgdir/usr/share/themes
	cp -r {buttons,GrayOrange} $pkgdir/usr/share/themes
}