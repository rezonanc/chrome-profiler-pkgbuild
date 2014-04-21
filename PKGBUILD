# Maintainer: Edvinas Aleksejonokas <rezonanc@gmail.com>

pkgname=chrome-profiler
pkgver=0.0.4
pkgrel=1
epoch=
pkgdesc="Chrome profile manager"
arch=(i686 x86_64)
url="https://github.com/rezonanc/chrome-profiler"
license=('GPL')
groups=()
depends=('coreutils' 'google-chrome')
makedepends=()
checkdepends=()
optdepends=()
provides=()
conflicts=()
replaces=()
backup=()
options=()
install=
changelog=
source=(https://github.com/rezonanc/$pkgname/archive/v$pkgver.tar.gz)
noextract=()
md5sums=('b635b26b733578be7cc99c1506745683')

package() {
	cd "$srcdir/$pkgname-$pkgver"
	
	install -D -m755 chrome-profile.sh $pkgdir/usr/bin/chrome-profile.sh
	install -D -m755 chrome-profiler_install.sh $pkgdir/usr/bin/chrome-profiler_install.sh
	install -D -m755 chrome-profiler_add.sh $pkgdir/usr/bin/chrome-profiler_add.sh
	install -D -m644 rebuild_profile_links.sh $pkgdir/usr/share/chrome-profiler/rebuild_profile_links.sh
}
