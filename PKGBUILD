# Maintainer: Rafael <rafael@rebornos.org>

pkgname=cnchi-mirrors
_pkgname=reborn-mirrorlist
_pkgname2=mirrorlist
pkgver=20210903
pkgrel=1
pkgdesc="RebornOS mirrors (reborn-mirrorlist and mirrorlist)"
arch=('any')
url="https://gitlab.com/rebornos-team/installers/cnchi/patches/cnchi-mirrors"
_url="https://gitlab.com/rebornos-team/rebornos-special-system-files/mirrors"
license=('GPL3')
source=("${_pkgname}"
        "${_pkgname2}")
sha256sums=('a6db2201c089f5b830061aaaebfe9835fcf1197405fea4e628910b4d709958ab'
            'f03a1b59ae6c9e5c7048c1417a0c60aed7cca22e018e40440a1224841d848df5')

pkgver() {
    date +%Y%m%d
}

package() {
    mkdir -p ${pkgdir}/home/rebornos/Downloads/
    install -Dm644 ${srcdir}/${_pkgname} ${pkgdir}/home/rebornos/Downloads/${_pkgname}
    install -Dm644 ${srcdir}/${_pkgname2} ${pkgdir}/home/rebornos/Downloads/${_pkgname2}
}
