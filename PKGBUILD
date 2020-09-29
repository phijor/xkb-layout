# Maintainer: Philipp Joram <philipp.joram at mailbox.tu-dresden.de>

pkgname=xkeyboard-layout-phijor
pkgver=1.2.1
pkgrel=1
pkgdesc='Xkeyboard US layout with German letters, phijor adaptions'
arch=(any)
license=(custom)
depends=('xkeyboard-config')

source=("phijor.xkb")
sha256sums=('c6c1cf95962891312805128a87fc62136d5e420cdef7829903be6157c45cd8bd')

package() {
    local _XKB_DIR="$pkgdir/usr/share/X11/xkb/symbols"
    install -v -m755 -d $_XKB_DIR
    install -v -m644 -D "phijor.xkb" "$_XKB_DIR/phijor"
}
