# Maintainer: Panda <panda@fydeos.io>

pkgname=fyde-keyring
pkgver=20240823
pkgrel=1
pkgdesc='Fyde PGP keyring'
arch=('any')
url='https://github.com/Linux-for-Fydetab-Duo/fyde-keyring'
license=('GPL')
install="${pkgname}.install"
source=('fyde.gpg'
        'fyde-revoked'
        'fyde-trusted')
md5sums=('59554d6d3032fe42d69d1e76e5b54b7f'
         'd41d8cd98f00b204e9800998ecf8427e'
         '7925623ace4b9cd8cddd1bfa556b4b37')

pkgver() {
    date +%Y%m%d
}

package() {
    cd "${srcdir}"
    install -Dm644 fyde.gpg "${pkgdir}/usr/share/pacman/keyrings/fyde.gpg"
    install -Dm644 fyde-revoked "${pkgdir}/usr/share/pacman/keyrings/fyde-revoked"
    install -Dm644 fyde-trusted "${pkgdir}/usr/share/pacman/keyrings/fyde-trusted"

}
