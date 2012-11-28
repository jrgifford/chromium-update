# Maintainer: Logan Allen <loganfynne at gmail dot com>
pkgname=chromium-update
pkgver=0.9
pkgrel=11
pkgdesc='Installer or updater of precompiled Chromium nightly builds'
arch=('any')
url="http://www.loganfynne.com/packages/chromium-update.tar"
license=('GPL')
conflicts=('chromium')
depends=('gconf' 'libpng12' 'gtk2' 'dbus-glib' 'nss' 'alsa-lib' 'xdg-utils' 'bzip2' 'libevent' 'libxss' 'libxtst' 'ttf-dejavu' 'desktop-file-utils' 'hicolor-icon-theme' 'unzip')
source=('http://www.loganfynne.com/packages/chromium-update.tar')
md5sums=('274d7db530d1f9bda12e0a7974bdb92a')

package() {
  tar -xf chromium-update.tar
  mkdir -p ${pkgdir}/usr/share/applications
  mkdir -p ${pkgdir}/usr/bin
  cp `arch`/chromium-update ${pkgdir}/usr/bin/
  chmod +x ${pkgdir}/usr/bin/chromium-update
  cp chromium.desktop ${pkgdir}/usr/share/applications/
  cp chromium ${pkgdir}/usr/bin/
}
