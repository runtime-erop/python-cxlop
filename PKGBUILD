pkgname=python-cxlop
pkgver=0.1.0
pkgrel=1
pkgdesc="LEV PROSHEL AVERNUS"
arch=('any')
url="https://github.com/runtime-erop/python-cxlop"
license=('MIT')
depends=('python')
makedepends=('python-setuptools')
source=("https://files.pythonhosted.org/packages/source/${pkgname#python-}/${pkgname#python-}/${pkgname#python-}-${pkgver}.tar.gz")
sha256sums=('abc123...')  # Replace with the actual SHA256 checksum

build() {
    cd "${srcdir}/${pkgname#python-}-${pkgver}"
    python setup.py build
}

package() {
    cd "${srcdir}/${pkgname#python-}-${pkgver}"
    python setup.py install --root="${pkgdir}" --optimize=1 --skip-build
}
