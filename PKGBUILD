# Maintainer: yozi <es.mslj TA xunilhcra> backwards
# Contributor: Bernd Amend <bernd.amend+extension_system gmail com>
pkgname='libcatch-cpp-headers'
pkgver=1.4.0
pkgrel=1
pkgdesc='C++-native framework for unit-tests using only a header file'
arch=(any)
url='http://catch-lib.net'
license=('custom:BSL')
source=('https://raw.githubusercontent.com/philsquared/Catch/v1.4.0/single_include/catch.hpp'
        'https://raw.githubusercontent.com/philsquared/Catch/v1.4.0/LICENSE_1_0.txt')
sha256sums=('c67e01b0f4c7617d6d695d14ad548e88b30cda178466c820ec9dc540d5e58bd9'
            'c9bff75738922193e67fa726fa225535870d2aa1059f91452c411736284ad566')

package() {
  install -D -m644 catch.hpp "${pkgdir}/usr/include/catch.hpp"
  install -D -m644 LICENSE_1_0.txt "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE"
}

# vim:set ts=2 sw=2 et:
