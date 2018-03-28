# Maintainer: manuel (see forum.antergos.com)

pkgdesc="Associate programs to filename extensions."
pkgname=assoc
pkgver=0.1.46
pkgrel=1
url="https://github.com/manuel-192/$pkgname"
arch=('any')
license=('GPL3')
depends=('bash')
source=(
  "$url/raw/master/$pkgname.bash-$pkgver"
)
sha512sums=(
  '4a5f72e4a8d5f9285b812e4ea5e9ee4e682de30a34144dfb00f40b79ce5434413a3842d507aaa50a585a43b94c7aa6848c6254b3074791111097089984bc03ba'
)

package() {
  cd $srcdir
  install -Dm555 $pkgname.bash-$pkgver $pkgdir/usr/bin/$pkgname.bash
}
