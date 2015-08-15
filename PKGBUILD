# Maintainer: jianqun <jianqun@chinesemail.net>

pkgname=greybird-themes
pkgver=20130712
pkgrel=1
pkgdesc="Desktop Suite for Xfce."
arch=('any')
url="https://github.com/shimmerproject/Greybird"
license=('GPL2' 'CCPL:cc-by-sa-3.0')
depends=('gtk-engine-murrine')
optdepends=('elementary-icon-theme: An icon theme designed to be smooth, sexy, clear, and efficient.')
conflicts=('xfce-theme-greybird' 'xfce-theme-greybird-git')
source=("http://cache.chinesehost.net/download/linux/$pkgname-$pkgver-$pkgrel.tar.gz")
md5sums=('733645c63c519a7677501d6154d6de10')

package() {
    cd "$srcdir/Greybird-master/"
    rm -f {.gitignore,LICENSE.{CC,GPL},README}
    install -d "$pkgdir/usr/share/themes/Greybird"
    cp -Rf . "$pkgdir/usr/share/themes/Greybird/"
}
