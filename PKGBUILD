# Maintainer: Matthew Phillip Cooper <matthew@coopertronic.co.uk>
pkgname=git-helper
_destname1="/usr"
pkgver=1
pkgrel=1
pkgdesc="Configation files that setup Calamares for Coopertronic OS"
arch=('any')
url="https://github.com/Coopertronic/ctos-calamares-settings.git"
license=('GPL2')
makedepends=('git')
depends=('git')
conflicts=()
provides=("${pkgname}")
options=(!strip !emptydirs)
source=("git+$url")
sha256sums=('SKIP')

pkgver() {
    printf "1.r%s.%s" "$(git rev-list --count HEAD)" "$(git rev-parse --short HEAD)"
}

package() {
	install -dm755 ${pkgdir}${_destname1}
	cp -r ${srcdir}/${pkgname}${_destname1}/* ${pkgdir}${_destname1}
}
