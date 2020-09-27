# Maintainer: Philipp Joram <philipp.joram at mailbox.tu-dresden.de>

pkgname=xkeyboard-layout-phijor
pkgver=1.2
pkgrel=1
pkgdesc='Xkeyboard US layout with German letters, phijor adaptions'
arch=(any)
license=(custom)
depends=('xkeyboard-config')

source=("phijor.xkb")
sha256sums=('d6b593c92a6f62f7b405e3a572a456d479c0c5590491fe1c525ed65234629e9f')

package() {
    local _XKB_DIR="$pkgdir/usr/share/X11/xkb/symbols"
    install -v -m755 -d $_XKB_DIR
    install -v -m644 -D "phijor.xkb" "$_XKB_DIR/phijor"
}
