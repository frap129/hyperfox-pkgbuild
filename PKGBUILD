# Maintainer: lsf

pkgname=librewolf-bin
provides=(${pkgname//-bin/""})
conflicts=(${pkgname//-bin/""})
_pkgname=LibreWolf
pkgver=70.0
pkgrel=1
_uploadh='329034521'
# _uploadpath="https://gitlab.com/${pkgname//-bin/""}-community/browser/arch/uploads/${_uploadh}/${pkgname//-bin/""}-${pkgver}-${pkgrel}-x86_64.pkg.tar.xz"
_uploadpath="https://gitlab.com/${pkgname//-bin/""}-community/browser/arch/-/jobs/${_uploadh}/artifacts/raw/${pkgname//-bin/""}-${pkgver}-${pkgrel}-x86_64.pkg.tar.xz"
pkgdesc="Community-maintained fork of Librefox: a privacy and security-focused browser"
arch=(x86_64)
license=(MPL GPL LGPL)
url="https://LibreWolf.gitlab.io"
depends=(gtk3 mozilla-common libxt startup-notification mime-types dbus-glib
         ffmpeg nss ttf-font libpulse)
optdepends=('networkmanager: Location detection via available WiFi networks'
            'libnotify: Notification integration'
            'pulseaudio: Audio support'
            'speech-dispatcher: Text-to-Speech'
            'hunspell-en_US: Spell checking, American English')
options=(!emptydirs)
install=librewolf-bin.install
source=(${_uploadpath})
sha256sums=('04d90cb051021248eda86d218b866947534ec360d095aa3d9a122914deb5868a')

package() {
  cp -r $srcdir/usr $pkgdir/
}
