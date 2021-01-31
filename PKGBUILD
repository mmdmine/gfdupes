#Maintainer: madamin <madamin@pm.me>
pkgname=gfdupes
pkgver=master
pkgrel=1
pkgdesc='A graphical frontend to fdupes, the utility to find duplicate files in a directory'
arch=(any)
license=(unknown)
url="https://github.com/mmdmine/gfdupes"
depends=(python pygtk fdupes)
source=(gfdupes.py)
md5sums=('9cca920e80fa97b9f4d0c5d318d487f5')
package()
{
	install -Dm644 "$srcdir/gfdupes.py" "$pkgdir/usr/bin/gfdupes"
	chmod +x "$pkgdir/usr/bin/gfdupes"
}
