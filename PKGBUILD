# $Id$
# Maintainer: Antoine Gagné <antoine.gagne.2@ulaval.ca>

pkgname=font-awesome
pkgver=1.0
_relver=2.010R-ro/1.030R-it
pkgrel=3
pkgdesc="Font Awesome taken from the popular web fonts at: http://fontawesome.io/."
url="https://github.com/AntoineGagne/font-awesome"
arch=(any)
license=(custom)
_tarname=font-awesome-${_relver//\//-}
source=("$_tarname.tar.gz::https://github.com/AntoineGagne/font-awesome/archive/$_relver.tar.gz")
sha256sums=('3ee5a0d04e6586f12de038cb33ec963f137bbc4907ae1e10a6333478a2b884f8')

package() {
  cd $_tarname
  install -d "$pkgdir/usr/share/fonts/${pkgname%-fonts}"
  install -t "$pkgdir/usr/share/fonts/${pkgname%-fonts}" -m644 OTF/*.otf
  install -Dm644 LICENSE.txt "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
}

# vim:set ts=4 sw=4 et:
