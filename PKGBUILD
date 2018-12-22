# Maintainer: William Luc Ritchie <luc dot ritchie at gmail dot com>

pkgname=xkb-programisto-dvorak
pkgver=1.1.1
pkgrel=1
pkgdesc='Dvorak-based xkb layout for programmers, with Esperanto keys'
arch=('any')
license=('custom')
source=('podvorak'
        '90-xkb-podvorak.conf'
        'UNLICENSE')
sha256sums=('312711da3edfc0f9aef4f1d8c31e2c57639ab37251cd57e942e54f51c8f7adcf'
            'e528d35ec6aa1c21cf64d9bb3906c4fddecc61bcfde28f404592c16fc0533962'
            '7e12e5df4bae12cb21581ba157ced20e1986a0508dd10d0e8a4ab9a4cf94e85c')

package() {
    cd "$srcdir"
    install -Dm644 'podvorak' "$pkgdir/usr/share/X11/xkb/symbols/podvorak"
    install -Dm644 '90-xkb-podvorak.conf' "$pkgdir/etc/X11/xorg.conf.d/90-xkb-podvorak.conf"
    install -Dm644 'UNLICENSE' "$pkgdir/usr/share/licenses/$pkgname/UNLICENSE"
}
