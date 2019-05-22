pkgname=python3-websockets
pkgver=7.0
pkgrel=1
pkgdesc='Library for building WebSocket servers and clients in Python'
arch=('x86_64')
url='https://websockets.readthedocs.io/'
license=('custom: BSD')
depends=('python3-setuptools')
source=("https://github.com/aaugustin/websockets/archive/${pkgver}.tar.gz")
md5sums=('a024bae83df5699a8bd490aee21b45be')

package() {
  cd websockets-${pkgver}
  
  python3 setup.py install --root=${pkgdir} --optimize=1
  
  install -D -m 644 LICENSE ${pkgdir}/usr/share/licenses/${pkgname}/LICENSE
}
