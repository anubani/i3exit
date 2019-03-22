# Maintainer: Ali Nubani <ali.alnubani94@gmail.com>

pkgname=i3exit
pkgver=20190322
pkgrel=1
pkgdesc="Systemd/OpenRC-compatible exit-script for i3, including 'blurlock'"
arch=('any')
license=('GPL')
depends=('i3-gaps'
    'i3lock'
    'imagemagick')
optdepends=('lightdm-gtk-greeter: switch user with lightdm')
source=("$pkgname"
    'blurlock')
md5sums=('SKIP')

pkgver() {
	date +'%Y%m%d'
}

package() {
	install -Dm755 $srcdir/$pkgname $pkgdir/usr/bin/i3exit
	install -Dm755 $srcdir/blurlock $pkgdir/usr/bin/blurlock
}
