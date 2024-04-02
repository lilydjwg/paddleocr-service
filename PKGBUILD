# Maintainer: lilydjwg <lilydjwg@gmail.com>
pkgname=paddleocr-config
pkgver=1.0
pkgrel=14
pkgdesc="Config paddleocr nspawn service"
arch=('any')
license=("BSD")
source=()
backup=(
  etc/systemd/nspawn/paddleocr.nspawn
  etc/systemd/nspawn/paddleocr-cpu.nspawn
  etc/nginx/conf.d/paddleocr.conf
)
optdepends=(
  'nginx: HTTP API for paddleocr-web'
)

build() {
  true
}
package() {
  cp -ar "$startdir"/root/* "${pkgdir}"
  find "${pkgdir}" -name '*~' -delete
}
