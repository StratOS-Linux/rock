pkgname=lugpkg
pkgver=1.0
pkgrel=0
pkgdesc="Package manager wrapper for lugOS"
arch=("any")
url="https://github.com/lugvitc/lugpkg"
license=('MIT')
depends=('bash')
optdepends=('yay-bin: AUR support'
	    'flatpak: Flatpak support'
	    'snapd: snap support'
	    )
source=("git+https://github.com/lugvitc/${pkgname}.git")
sha1sums=('SKIP')

package() {
    cd "$pkgname"
    mkdir -p $pkgdir/usr/bin
    install -D -m755 ./lugpkg $pkgdir/usr/bin/$pkgname
}
