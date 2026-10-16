# Maintainer: Clément Foucher <cfoucher-pkg at outlook dot fr>
pkgname=pacman-reminder
pkgver=0.0.1
pkgrel=1
pkgdesc="A reminder for updating Pacman"
arch=('x86_64')
url="https://github.com/ClementFoucher/pacman-reminder"
license=('GPL-2.0-or-later')
depends=()
makedepends=()
source=("https://raw.githubusercontent.com/ClementFoucher/pacman-reminder/refs/heads/main/pacman-reminder.py"
        "https://raw.githubusercontent.com/ClementFoucher/pacman-reminder/refs/heads/main/pacman-reminder.conf"
       )
sha256sums=('1d2e0e2e2761b39cbc77e5d86a0f8f6f6c40c4e2b3a2ed3be7755f7be2b49bcc'
            '15cb3c8a84b36bf721166a828823fb3de2a3bc799ceca26c7768eb55e1cc60b4')
package() {
        mkdir "$pkgdir/usr"

        mkdir "$pkgdir/usr/bin"
        install "$srcdir/pacman-reminder.py" "$pkgdir/usr/bin/pacman-reminder"

		mkdir "$pkgdir/usr/share"
        install "$srcdir/pacman-reminder.conf" "$pkgdir/usr/share/"
}
