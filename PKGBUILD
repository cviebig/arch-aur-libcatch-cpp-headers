# Maintainer: yozi <es.mslj TA xunilhcra> backwards
# Contributor: Bernd Amend <bernd.amend+extension_system gmail com>
pkgname='libcatch-cpp-headers'
pkgver=1.9.3
pkgrel=2
pkgdesc='C++-native framework for unit-tests using only a header file'
arch=(any)
url='http://catch-lib.net'
license=('custom:BSL')
source=("https://raw.githubusercontent.com/philsquared/Catch/v${pkgver}/single_include/catch.hpp"
        "LICENSE::https://raw.githubusercontent.com/philsquared/Catch/v${pkgver}/LICENSE.txt")
sha256sums=('add614987e6215a2a095410765f5e5ac17f3b4f4019e9aad01e49a551b9f03ea'
            'c9bff75738922193e67fa726fa225535870d2aa1059f91452c411736284ad566')

pkgver() {
  echo $(grep -oEm1 \
    '^.*Catch v[0-9]\.[0-9]+\.[0-9]+$' \
    catch.hpp | cut -d'v' -f2)
}

package() {
  install -D -m644 catch.hpp "${pkgdir}/usr/include/catch.hpp"
  install -D -m644 LICENSE "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE"
}

# vim:set ts=2 sw=2 et:
