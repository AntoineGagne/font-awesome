# $Id$
# Maintainer: Antoine Gagné <antoine.gagne.2@ulaval.ca>

pkgname=font-awesome
pkgver=1.0
_relver=1.0
pkgrel=3
pkgdesc="Font Awesome taken from the popular web fonts at: http://fontawesome.io/."
url="https://github.com/AntoineGagne/font-awesome"
arch=(any)
license=(custom)
_tarname=font-awesome-${_relver//\//-}
source=("$_tarname.tar.gz::https://github.com/AntoineGagne/font-awesome/archive/$_relver.tar.gz")

package() {
  cd $_tarname
  install -d "$pkgdir/usr/share/fonts/${pkgname%-fonts}"
  install -t "$pkgdir/usr/share/fonts/${pkgname%-fonts}" -m644 OTF/*.otf
  install -Dm644 LICENSE.txt "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
}

# vim:set ts=4 sw=4 et:
