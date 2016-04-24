#Maintainer: Alex Gajewski <agajews@gmail.com>

_pkgname='Apricity Themes'
pkgname=apricity-themes-gnome
pkgver=1.0.1
pkgrel=1
pkgdesc='Gnome Assets for Apricity OS'
arch=(any)
license=(GPL)
url="https://github.com/Apricity-OS/apricity-themes-gnome"
depends=()
replaces=(apricity-themes)
conflicts=(apricity-themes, apricity-themes-cinnamon)
provides=(apricity-themes)
source=("apricity-themes-gnome.tar.gz")
sha256sums=('1c500f365b7ceea2092ab1eefef149c73137cd0067c101119e4504bf7b11b619')
install="apricity-themes-gnome.install"

package() {
	rm -rf "${pkgdir}/usr/share/themes/Arctic Apricity"
	mkdir -p "${pkgdir}/usr/share/themes"
	mkdir -p "${pkgdir}/etc/skel/.config/autostart"
	cp -rf "${srcdir}/apricity-themes-gnome/Arctic Apricity" "${pkgdir}/usr/share/themes"
	cp -f "${srcdir}/apricity-themes-gnome/firstrun-desktop.sh" "${pkgdir}/etc/skel/.config/autostart"
}
