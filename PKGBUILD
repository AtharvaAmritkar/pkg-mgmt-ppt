# Maintainer: Atharva Amritkar <atharvaamritkar@protonmail.com>
pkgname=sampleprog
pkgver=1.0.0
pkgrel=1
pkgdesc="A sample c program"
arch=("x86_64")
url="https://gitlab.com/AtharvaAmritkar/sampleprog"
license=('MIT')
depends=(gcc)
makedepends=(git)

source=("git+$url.git")
md5sums=( 'SKIP')

build() {
	cd sampleprog
	gcc asd.c -Wall -Wextra -Wpedantic -Wshadow -O3 -o mylovelyprogram
}

package() {
	cd sampleprog
        install -Dm 755 mylovelyprogram $pkgdir/usr/bin/mylovelyprogram
}
