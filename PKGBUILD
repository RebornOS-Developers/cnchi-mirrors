# Maintainer: Rafael <rafael@rebornos.org>

pkgname=cnchi-mirrors
_pkgname=reborn-mirrorlist
_pkgname2=mirrorlist
pkgver=20210609
pkgrel=1
pkgdesc="RebornOS mirrors (reborn-mirrorlist and mirrorlist)"
arch=('any')
url="https://gitlab.com/rebornos-team/installers/cnchi/patches/cnchi-mirrors"
_url="https://gitlab.com/rebornos-team/rebornos-special-system-files/mirrors"
license=('GPL3')
source=("${_url}/${_pkgname}/-/raw/master/${_pkgname}"
        "${_url}/${_pkgname2}/-/raw/master/${_pkgname2}")
sha256sums=('1405e2bace22ee072e598a8549976be5b0bd1dbcda0d50f98b37d176b260d4b7'
            '6fb580a546a2b00ec705b97e9f6f2dcccc139714f0e795d2f5e7aa6f57323174')

pkgver() {
    date +%Y%m%d
}

package() {
    mkdir -p ${pkgdir}/home/rebornos/Downloads/
    install -Dm644 ${srcdir}/${_pkgname} ${pkgdir}/home/rebornos/Downloads/${_pkgname}
    install -Dm644 ${srcdir}/${_pkgname2} ${pkgdir}/home/rebornos/Downloads/${_pkgname2}
}
