# Maintainer: satya164
# Contributor: benwbooth
pkgname='gtk-theme-ambiance-blue'
pkgver=2012.05.30
pkgrel=1
pkgdesc="Ambiance Blue is a bluish variant of the Ambiance theme compatible with both Gnome Shell and Unity."
arch=(any)
url="http://satya164.deviantart.com/art/Ambiance-Blue-Theme-Suite-196833665"
license=('GPL')
depends=('gtk-engine-unico' 'gtk-engine-murrine')
conflicts=()
source=('http://www.deviantart.com/download/196833665/ambiance_blue_theme_suite_by_satya164-d396ttt.zip')
md5sums=('6cb8db2f7c167b544a4805604ba46659')
install=

package() {
 	bsdtar -xf ${srcdir}/ambiance_blue_theme_suite_by_satya164-d396ttt.zip
	mkdir -p ${pkgdir}/usr/share/themes
	cp -R ${srcdir}/Ambiance*  ${pkgdir}/usr/share/themes/
	cd ${pkgdir}/usr/share/themes/
	find . -type f -exec chmod 644 {} \;
	find . -type d -exec chmod 755 {} \;
}
