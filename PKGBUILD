# $Id$
# Maintainer: Antoine Gagné <antoine.gagne.2@ulaval.ca>

pkgname=font-awesome
pkgver=1.0.2
_relver='v4.7.0'
pkgrel=3
pkgdesc="Font Awesome taken from the popular web fonts at: http://fontawesome.io/."
url="https://github.com/AntoineGagne/font-awesome"
arch=(any)
license=(custom)
_tarname=Font-Awesome-${_relver#?}
md5sums=('a6145901f233f7d54165d8ade779082e')
source=("$_tarname.tar.gz::https://github.com/FortAwesome/Font-Awesome/archive/$_relver.tar.gz")

package() {
    cd $_tarname
    install -d "$pkgdir/usr/share/fonts/${pkgname%-fonts}"
    install -t "$pkgdir/usr/share/fonts/${pkgname%-fonts}" -m644 fonts/*.otf
}

# vim:set ts=4 sw=4 et:
