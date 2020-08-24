pkgname=powertune
pkgver=0.0.1
pkgrel=1
pkgdesc="Run powertop autotune at boot"
url="https://github.com/kevinschoon/powertune"
arch=(x86_64)
license=('MIT')
md5sums=()
validpgpkeys=()

build() {
	cp ../powertune .
	cp ../powertune.service .
}

package() {
	install -Dm755 "powertune" -t "${pkgdir}"/usr/bin/
	install -Dm644 "powertune.service" -t ${pkgdir}/usr/lib/systemd/system/
}
