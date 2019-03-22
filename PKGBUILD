# Maintainer: Ali Nubani <ali.alnubani94@gmail.com>

pkgname=i3exit
pkgver=20180529
pkgrel=1
pkgdesc="Systemd/OpenRC-compatible exit-script for i3, including 'blurlock'"
arch=('any')
groups=('i3-manjaro')
license=('GPL')
depends=('i3-wm'
    'i3lock'
    'imagemagick')
optdepends=('lightdm-gtk-greeter: switch user with lightdm')
source=("$pkgname"
    'blurlock')
md5sums=('cf20f699b2cdc2fb7d22075866e54a9f'
         'e3699b2b3acaa6e59e4d40d9229273ea')

pkgver() {
	date +'%Y%m%d'
}

package() {
	install -Dm755 $srcdir/$pkgname $pkgdir/usr/bin/i3exit
	install -Dm755 $srcdir/blurlock $pkgdir/usr/bin/blurlock
}
