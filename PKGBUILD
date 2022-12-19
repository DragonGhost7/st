# Maintainer: Me lmao
pkgname="st"
pkgver=r1166.856a42f
groups=('modified')
pkgrel=1
pkgdesc="suckless terminal"
arch=('x86_64')
url='git.suckless.org/st'
license=('MIT')
depends=('libxft-bgra')
makedepends=('git')
optdepends=('xurls: for copying output',
			'xargs: for copying output')
source=('st::git://github.com/DragonGhost7/st.git')
md5sums=('SKIP')

pkgver() {
cd "$pkgname"
printf "r%s.%s" "$(git rev-list --count HEAD)" "$(git rev-parse --short HEAD)"
}

build() {
	cd "$pkgname"
	make
}

package() {
	cd "$pkgname"
	install -Dm755 ./st "$pkgdir/usr/local/bin/st"
	install -Dm644 ./st.1 "$pkgdir/usr/local/man/man1/st.1"
	install -Dm644 ./st.desktop "$pkgdir/usr/local/share/applications/st.desktop"
}
