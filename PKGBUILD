# Maintainer: manuel (see forum.antergos.com)

pkgdesc="Associate programs to filename extensions."
pkgname=assoc
pkgver=0.1.43
pkgrel=1
url="https://github.com/manuel-192/$pkgname"
arch=('any')
license=('GPL3')
depends=('bash')
source=(
  "$url/raw/master/$pkgname.bash-$pkgver"
)
sha512sums=(
  '3e7651f800a4a480142b7fa6e01ecff5dc9b85479598e025136b8d34ebf1e0a1ad1325a3026030a4be559d721c35c432074b31b071ca2ee7fc9758d445efbbd1'
)

package() {
  cd $srcdir
  install -Dm555 $pkgname.bash-$pkgver $pkgdir/usr/bin/$pkgname.bash
}
