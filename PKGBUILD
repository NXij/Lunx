# Trillian IM client
# Precompiled, propietary

pkgname=trillian
pkgver=2.0.0.4
pkgrel=1
pkgdesc="A commercial, multi-protocol and cross-platform IM client"
arch=('i686' 'x86_64')
url="https://www.trillian.im"
license=('Proprietary')
depends=('gtkmm3' 'libzip' 'openssl' 'webkitgtk' 'libnotify' 'libpulse' 'libxss')
install='trillian.install'
 
if [[ "$CARCH" == "i686" ]]; then
	source=("https://www.trillian.im/get/linux/2.0/apt/dists/stable/main/binary-i386/trillian_2.0.0.4_i386.deb")
	sha256sums=('f801dab0a879f6496dd4d37aded8c1532b015313f69080e865a34b6d108b8058')
elif [[ "$CARCH" == "x86_64" ]]; then
	source=("https://www.trillian.im/get/linux/2.0/apt/dists/stable/main/binary-amd64/trillian_2.0.0.4_amd64.deb")
	sha256sums=('2096b8de7db16d917a75c932ee5b0889a08264b06bc7b20dc1d17c657b5a6844')
fi
 
package() {
  tar xzvf "$srcdir/data.tar.gz" -C "$pkgdir/"
}