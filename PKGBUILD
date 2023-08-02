# Maintainer: Matthew Phillip Cooper <matthew@coopertronic.co.uk>
pkgname=git-helper
_destname1="/usr"
pkgver=1.r7.8a6c9f2
pkgrel=1
pkgdesc="Helper scripts that make using git in CLI less time consuming."
arch=('any')
url="https://github.com/Coopertronic/git-helper.git"
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
