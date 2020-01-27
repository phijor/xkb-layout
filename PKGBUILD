# Maintainer: Philipp Joram <philipp.joram at mailbox.tu-dresden.de>

pkgname=xkeyboard-layout-phijor
pkgver=1.0
pkgrel=1
pkgdesc='Xkeyboard US layout with German letters, phijor adaptions'
arch=(any)
license=(custom)
depends=('xkeyboard-config')

source=("phijor.xkb")
sha256sums=('c8450fa7fc34793de7cbeef97cf9995230d51c7693947f36c6e356cc8fb635f4')

package() {
    local _XKB_DIR="$pkgdir/usr/share/X11/xkb/symbols"
    install -v -m755 -d $_XKB_DIR
    install -v -m644 -D "phijor.xkb" "$_XKB_DIR/phijor"
}
