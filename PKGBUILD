# Maintainer: William Luc Ritchie <luc dot ritchie at gmail dot com>

pkgname=xkb-programisto-dvorak
pkgver=1
pkgrel=1
pkgdesc='Dvorak-based xkb layout for programmers, with Esperanto keys'
arch=('any')
license=('custom')
source=('podvorak'
        '90-xkb-podvorak.conf'
        'LICENSE')
sha256sums=('5083880c85e50d8cb7b7f7d98c254615f11e5bd5003a838648f87f9c79bf17bf'
            'e528d35ec6aa1c21cf64d9bb3906c4fddecc61bcfde28f404592c16fc0533962'
            'f2fd10444bf730e5d03c46211981c11ad8c3ec71e2564075eb28fbfd9b90e1fb')

package() {
    cd "$srcdir"
    install -Dm644 'podvorak' "$pkgdir/usr/share/X11/xkb/symbols/podvorak"
    install -Dm644 '90-xkb-podvorak.conf' "$pkgdir/etc/X11/xorg.conf.d/90-xkb-podvorak.conf"
    install -Dm644 'LICENSE' "$pkgdir/usr/share/licenses/xkb-programisto-dvorak/LICENSE"
}
