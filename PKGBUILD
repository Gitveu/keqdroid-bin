# Maintainer: Cybertveu cybertveu@gmail.com
pkgname=keqdroid-bin
pkgver=0.37.4
pkgrel=1
pkgdesc="Material 3 proxy and VPN client supporting Sing-box, Xray and Mihomo"
arch=('x86_64')
url="https://github.com/Lemonochka/keqdroid"
license=('GPL-3.0-or-later')
depends=(
    'at-spi2-core'
    'cairo'
    'fontconfig'
    'gdk-pixbuf2'
    'gtk3'
    'harfbuzz'
    'hicolor-icon-theme'
    'libayatana-appindicator'
    'libepoxy'
    'pango'
)
optdepends=(
    'polkit: TUN mode authentication agent'
    'zenity: GUI dialogs'
    'xdg-desktop-portal-gtk: desktop portal backend'
    'xdg-desktop-portal-kde: desktop portal backend for KDE'
    'xdg-desktop-portal-gnome: desktop portal backend for GNOME'
    'gnome-shell-extension-appindicator: tray icon support for GNOME'
)
provides=("${pkgname%-bin}")
conflicts=("${pkgname%-bin}")
source=("${pkgname}-${pkgver}.deb::https://github.com/Lemonochka/keqdroid/releases/download/v${pkgver}/keqdroid_${pkgver}_amd64.deb")
sha256sums=('89e4c57f1256f1dda7a3c303366a76537a5a04c5d31c4f312ea0662f37f9c3b6')

package() {
    ar x "${srcdir}/${pkgname}-${pkgver}.deb"
    bsdtar -xf data.tar.* -C "${pkgdir}"

    find "${pkgdir}" -type d -exec chmod 755 {} +
    find "${pkgdir}/usr/share" -type f -exec chmod 644 {} + 2>/dev/null || true
    if [ -d "${pkgdir}/usr/bin" ]; then
        chmod 755 "${pkgdir}/usr/bin/"* 2>/dev/null || true
    fi
}
