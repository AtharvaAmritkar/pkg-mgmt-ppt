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
	gcc asd.c -o mylovelyprogram
}

package() {
	cd sampleprog
#if you are facing issue during install ,add comment on line 23 and remove comment from line 24
 install -Dm 755 mylovelyprogram $pkgdir/usr/bin/mylovelyprogram
#sudo cp mylovelyprogram /usr/bin
}
#type 'mylovelyprogram' in your terminal to run the installled package
