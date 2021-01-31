#Maintainer: madamin <madamin@pm.me>
pkgname=gfdupes
pkgver=master
pkgrel=1
pkgdesc='A graphical frontend to fdupes, the utility to find duplicate files in a directory'
arch=(any)
license=(unknown)
url="https://github.com/mmdmine/gfdupes"
depends=(python pygtk gtk3 fdupes)
source=(gfdupes.py)
md5sums=('53ff7df0873521248d36d2bbcfbc7686')
package()
{
	install -Dm644 "$srcdir/gfdupes.py" "$pkgdir/usr/bin/gfdupes"
	chmod +x "$pkgdir/usr/bin/gfdupes"
}
