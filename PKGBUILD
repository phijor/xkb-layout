# Maintainer: Philipp Joram <philipp.joram at mailbox.tu-dresden.de>

pkgname=xkeyboard-layout-phijor
pkgver=1.3.1
pkgrel=1
pkgdesc='Xkeyboard US layout with German letters, phijor adaptions'
arch=(any)
license=(custom)
depends=('xkeyboard-config')

source=("phijor.xkb")
sha256sums=('2b4459550b1587b3bf80a8a205b349c44630ba0953df2eb5f8a5a660ff466837')

package() {
    local _XKB_DIR="$pkgdir/usr/share/X11/xkb/symbols"
    install -v -m755 -d $_XKB_DIR
    install -v -m644 -D "phijor.xkb" "$_XKB_DIR/phijor"
}
