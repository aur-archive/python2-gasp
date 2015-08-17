# Maintainer: Connor Behan <connor.behan@gmail.com>
# Contributor: Christoph Zeiler <rabyte*gmail>
# Contributor: Thomas Dziedzic

pkgname=python2-gasp
pkgver=0.3.4
pkgrel=1
pkgdesc="Procedural API for beginning programmers built on the PyCairo library"
arch=('any')
url="https://launchpad.net/gasp-core"
license=('GPL3')
depends=('pygtk')
makedepends=('python2-distribute')
replaces=('python-gasp')
source=(http://launchpad.net/gasp-core/0.3.x/$pkgver/+download/${pkgname#python2-}-${pkgver}.tar.gz)

package() {
  cd "${srcdir}"/${pkgname#python2-}-${pkgver}
  python2 setup.py install --root="${pkgdir}"
  rm -rf "${pkgdir}"/usr/lib/python*/site-packages/*.egg-info
}

md5sums=('59b4fbaa3f5bdf180dc1c2262a2258d7')
