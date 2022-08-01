# Contributor:
# Maintainer:
pkgname=bgs
pkgver=0.8
pkgrel=0
pkgdesc="background setter"
url="https://github.com/Gottox/bgs/"
arch="all"
license="MIT"
depends="libx11 libxinerama imlib2"
makedepends="libx11-dev libxinerama-dev imlib2-dev"
subpackages="$pkgname-doc"
source="https://tmpfiles.org/dl/171832/$pkgname-$pkgver.tar.gz"
builddir="$srcdir/$pkgname-$pkgver/"
options="!check"

prepare() {
	default_prepare
}

build() {
	cd "$builddir"
	make
}

package() {
	cd "$builddir"
	make DESTDIR="$pkgdir" install
}

sha512sums="
82edfad9e3f56ca2b4f0a70e0be8d9d613a3524e8b48bf009d60770c4768f401c21614cad2e243998d1b96f4bca7f9ce6d58b5ec558b08f8b15eb688a0822185  bgs-0.8.tar.gz
"
