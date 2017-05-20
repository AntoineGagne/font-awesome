# $Id$
# Maintainer: Antoine Gagné <antoine.gagne.2@ulaval.ca>

pkgname=font-awesome
pkgver=1.0.1
_relver='v1.0.1'
pkgrel=3
pkgdesc="Font Awesome taken from the popular web fonts at: http://fontawesome.io/."
url="https://github.com/AntoineGagne/font-awesome"
arch=(any)
license=(custom)
_tarname=font-awesome-${_relver#?}
md5sums=('7a7bf54a401def4dba82aa60b3c9275b')
source=("$_tarname.tar.gz::https://github.com/AntoineGagne/font-awesome/archive/$_relver.tar.gz")

package() {
    cd $_tarname
    install -d "$pkgdir/usr/share/fonts/${pkgname%-fonts}"
    install -t "$pkgdir/usr/share/fonts/${pkgname%-fonts}" -m644 OTF/*.otf
    install -Dm644 LICENSE.txt "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
}

# vim:set ts=4 sw=4 et:
