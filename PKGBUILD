
pkgname=alterlinux_tui_installer
pkgver="0.0.1.$(date +%Y%m%d%H%M)"
pkgrel=1
pkgdesc="Alter Linux TUI Installer"
arch=('any')
depends=('python' 'dialog' 'python-pythondialog' 'gptfdisk')
makedepends=('python-setuptools')
source=("git+https://github.com/FascodeNet/AlterLinux-TUI-Installer.git")
sha512sums=('SKIP')

build() {
  cd AlterLinux-TUI-Installer
  python setup.py build
}

package() {
  cd AlterLinux-TUI-Installer
  python setup.py install --root="$pkgdir" --optimize=1 --skip-build
}
