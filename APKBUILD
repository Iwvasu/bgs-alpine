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
source="$pkgname-$pkgver.tar.gz::https://github.com/Gottox/bgs/archive/refs/tags/v$pkgver.tar.gz"
options="!check"

build() {
	cd "$builddir"
	make
}

package() {
	cd "$builddir"
	make PREFIX=/usr DESTDIR="$pkgdir" install
}

sha512sums="
4f7aa32d9cf60252abfc87cf72c7bc20ac691af3684a0923d3e2a3506407bddee9d2e5f49da97a154ed2acf1a876b2952ab61dd412f2de39c1303e7551acaec8  bgs-0.8.tar.gz
"
