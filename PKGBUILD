# Maintainer: Giorgio Gilestro <giorgio@gilest.ro>
pkgname=bbcrust
_pkgname=bbCrust
pkgver=0.1.0
pkgrel=3
pkgdesc="A modified version of python shell pyCrust"
arch=('i686' 'x86_64')
url="http://wxpython-users.1045709.n5.nabble.com/Re-PyCrust-Some-enhancements-Any-interest-td2331787.html"
license=('GPL')
depends=('python2' 'wxpython')
source=(http://gilest.ro/download/various/software/$_pkgname/$_pkgname-$pkgver.tar.gz)
md5sums=('6a5281122a77246f76de1aa996c4ae4b')

build() {
  cd "$srcdir/$_pkgname-$pkgver"
  install -d $pkgdir/usr/lib/share/bbCrust
  install -d $pkgdir/usr/bin
  install -d $pkgdir/usr/share/applications
  install *.py $pkgdir/usr/lib/share/bbCrust/
  install *.svg $pkgdir/usr/lib/share/bbCrust/
  install bbcrust.desktop $pkgdir/usr/share/applications/
  install -m755 bbCrust $pkgdir/usr/bin/
  
}
