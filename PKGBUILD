# Maintainer: Erik Dubois <erik.dubois@gmail.com>
pkgname=3xitlights-eyecandy
pkgver=1.0
pkgrel=1
_destname="/usr/share/icons/"
pkgdesc="3xitlights fav eyecandy"
arch=('any')
url="https://github.com/3xitlight/${pkgname}"
license=('Attribution-NonCommercial-ShareAlike 4.0 International Public License')
makedepends=('git')
provides=("${pkgname}")
conflicts=("${pkgname}")
options=(!strip !emptydirs)
source=(3xitlights-eyecandy::"https://github.com/3xitlight/archive/${pkgname}-${pkgver}-${pkgrel}.tar.gz")
sha256sums=('SKIP')
package() {
	find ${srcdir} -type f -name "*.sh" -exec chmod 644 '{}' \;
	install -dm 755 ${pkgdir}${_destname}
	rm ${srcdir}/${pkgname}
  	cp -r ${srcdir}/* ${pkgdir}${_destname}
}
