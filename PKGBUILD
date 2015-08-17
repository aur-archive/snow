# Maintainer: nil0x42 <http://goo.gl/kb2wf>
pkgname=snow
pkgver=20130616
pkgrel=3
pkgdesc="Steganography program for concealing messages in text files"
arch=('i686' 'x86_64')
url="http://web.archive.org/web/20140225172531/http://www.darkside.com.au/snow/"
license=('GPL')
makedepends=('make')
source=("http://web.archive.org/web/20140225172531/http://www.darkside.com.au/${pkgname}/${pkgname}-${pkgver}.tar.gz")
md5sums=('be8a28b7fb6e2c751fde7c0cc8ae01ec')

build() {
    cd "${srcdir}/${pkgname}-${pkgver}"
    make
}

package() {
    cd "${srcdir}/${pkgname}-${pkgver}"
    install -Dm755 snow "${pkgdir}/usr/bin/${pkgname}"
    install -Dm644 snow.1 "${pkgdir}/usr/share/man/man1/${pkgname}.1"
}
