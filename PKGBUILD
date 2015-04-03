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
 
if [[ "$CARCH" == "i686" ]]; then
	source=("https://www.trillian.im/get/linux/2.0/apt/dists/stable/main/binary-i386/trillian_2.0.0.4_i386.deb")
	sha256sums=('49EB59B9DC6D87CD6B2495D517B89ADFCA4B81265904A7F4B086663F6A3FA637')
elif [[ "$CARCH" == "x86_64" ]]; then
	source=("https://www.trillian.im/get/linux/2.0/apt/dists/stable/main/binary-amd64/trillian_2.0.0.4_amd64.deb")
	sha256sums=('E7F4F101F5C8B6D9E65244E47EAF38417B6486608EAF287DF7EAABE27B28FE0A')
fi
 
package() {
  tar xzvf "$srcdir/data.tar.gz" -C "$pkgdir/"
}