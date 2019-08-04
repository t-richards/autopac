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
            '5de1b6d33ed1786e172e576d50c6d4ca1843cf91fc9308e95d288400735d7305')

package() {
  install -d -m 755 "$pkgdir/usr/lib/systemd/system/"

  install -Dm644 autopac.{timer,service} "$pkgdir/usr/lib/systemd/system/"
}
