# Maintainer: ArchLatam <corelinuxx@gmail.com>

pkgname=calamares-config
pkgver=2.1
pkgrel=11
pkgdesc="Calamares configuration for Arch Linux Plasma"
arch=('any')
url="https://github.com/archlatam/calamares-config"
license=('custom')
makedepends=('git')
provides=("${pkgname}")
options=(!strip !emptydirs)

source=("${pkgname}::git+${url}#commit=HEAD")
sha256sums=('SKIP')

package() {
  # Instalar en /etc
  install -d "${pkgdir}/etc"

  # Copiar toda la carpeta /etc del repo
  cp -a "${srcdir}/${pkgname}/etc/." "${pkgdir}/etc/"
}
