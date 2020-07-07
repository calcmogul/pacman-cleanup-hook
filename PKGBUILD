# Maintainer: KopfKrieg <archlinux [at] absolem [dot] cc>

pkgname=pacman-cleanup-hook
pkgver=1.0
pkgrel=8
pkgdesc='Pacman hook to cleanup pacman cache, keeping only the latest cache and the currently installed package.'
arch=('any')
depends=('pacman-contrib')
source=('cleanup.hook' 'remove-uninstalled.hook')
sha256sums=('52c6bcbdc0acf7dab8c4a5f1c1e60589d30d1b244016562431b53e7710c5784a'
            '00d2bcb94c65049b5753c1340c09a9a03869793de97400a222adb203f374d97f')

package() {
  install -D -m0644 "${srcdir}/cleanup.hook" "${pkgdir}/usr/share/libalpm/hooks/cleanup.hook"
  install -D -m0644 "${srcdir}/remove-uninstalled.hook" "${pkgdir}/usr/share/libalpm/hooks/remove-uninstalled.hook"
}
