# Maintainer: manuel (see forum.antergos.com)

pkgdesc="Associate programs to filename extensions."
pkgname=assoc
pkgver=0.1.47
pkgrel=1
url="https://github.com/manuel-192/$pkgname"
arch=('any')
license=('GPL3')
depends=('bash')
source=(
  "$url/raw/master/$pkgname.bash-$pkgver"
)
sha512sums=(
  '200d5e9c253dfa28fe939447a29a31d2587e9ecd5995d8220858fdb7644acd0782f7a34ccad686e0101d7cec3c7eddf6afa24f1719fabb68ed1b1e0ac7b38059'
)

package() {
  cd $srcdir
  install -Dm555 $pkgname.bash-$pkgver $pkgdir/usr/bin/$pkgname
}
