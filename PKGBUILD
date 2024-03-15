# Maintainer: Tom Richards <tom@tomrichards.net>

pkgname=autopac
pkgver=1.0.0
pkgrel=1
pkgdesc='Automatically download package updates'
arch=('any')
url='https://github.com/t-richards/autopac'
license=('MIT')
install=autopac.install
source=(autopac.timer
        autopac.service)
sha256sums=('a7d198e4ad9075b41a7583403ffa31e415cd7e428cb03f762fac482e3e948673'
            '2d0d649ff5691bd4fc32efcd5ad7f9099de62062f42be2da46c680c560346abb')

package() {
  install -d -m 755 "$pkgdir/usr/lib/systemd/system/"

  install -Dm644 autopac.{timer,service} "$pkgdir/usr/lib/systemd/system/"
}
