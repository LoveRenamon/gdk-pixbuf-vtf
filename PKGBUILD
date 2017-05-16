pkgname=gdk-pixbuf-vtf
pkgver=20170516
pkgrel=1
pkgdesc='VTF GDK Pixbuf Loader library'
arch=('x86_64' 'i686')
url='https://github.com/Rahix/gdk-pixbuf-vtf'
depends=('gdk-pixbuf2')
makedepends=('cmake')
source=("git+https://github.com/Rahix/gdk-pixbuf-vtf.git#commit=61c19b1854ef50f9ba34322423aa0e4f858962ea")
sha256sums=('SKIP')

build() {
  cd "$pkgname"
  mkdir -p build && cd build
  cmake -DCMAKE_INSTALL_PREFIX:STRING=/usr ..
  make pixbufloader-vtf
}

package() {
  cd "$pkgname"/build
  make DESTDIR="$pkgdir/" install/fast
}
