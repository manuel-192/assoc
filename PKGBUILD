# Maintainer: manuel (see forum.antergos.com)

pkgdesc="Associate programs to filename extensions."
pkgname=assoc
pkgver=0.1.38
pkgrel=1
url="https://github.com/manuel-192/$pkgname"
arch=('any')
license=('GPL3')
depends=('bash')
source=(
  "$url/raw/master/$pkgname.bash-$pkgver"
)
sha512sums=(
  '861fc5d0f9a97c413a53bece817bc751ab5ba3906357a84bc5695071509b0216de2be4c8b6341d9a404abbcf2d2099a85109c9ec9273254b8941fd8d4238fcf6'
)

package() {
  cd $srcdir
  install -Dm555 $pkgname.bash-$pkgver $pkgdir/usr/bin/$pkgname.bash
}
