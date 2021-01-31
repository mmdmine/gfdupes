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
md5sums=('05be52a0f6731ec62ec607903d86053a')
package()
{
	install -Dm644 "$srcdir/gfdupes.py" "$pkgdir/usr/bin/gfdupes"
	chmod +x "$pkgdir/usr/bin/gfdupes"
}
