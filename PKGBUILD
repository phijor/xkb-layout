# Maintainer: Philipp Joram <philipp.joram at mailbox.tu-dresden.de>

pkgname=xkeyboard-layout-phijor
pkgver=1.2.2
pkgrel=1
pkgdesc='Xkeyboard US layout with German letters, phijor adaptions'
arch=(any)
license=(custom)
depends=('xkeyboard-config')

source=("phijor.xkb")
sha256sums=('947b67415ae6177a6614c8ed2dfbc36926ab9bd0b1f2d40531e3f5fae406419a')

package() {
    local _XKB_DIR="$pkgdir/usr/share/X11/xkb/symbols"
    install -v -m755 -d $_XKB_DIR
    install -v -m644 -D "phijor.xkb" "$_XKB_DIR/phijor"
}
