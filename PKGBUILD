# Maintainer: Gordin <9ordin @t gmail dot com>
# Generated by gem2arch

_gemname=lolcat
pkgname=$_gemname
pkgver=42.1.0
pkgrel=3
pkgdesc="Okay, no unicorns. But rainbows!!"
arch=('any')
url="https://github.com/busyloop/lolcat"
license=('custom')
depends=('ruby' 'ruby-paint>=0.8.3' 'ruby-trollop1>=1.16.2')
makedepends=('rubygems')
source=(http://rubygems.org/downloads/$_gemname-$pkgver.gem)
noextract=($_gemname-$pkgver.gem)
md5sums=('4924bc374f141019ad202cfb7b65bbd4')
sha1sums=('80151b3833bb7c19f5529e774366119879dbf204')

package() {
  cd "$srcdir"
  local _gemdir="$(ruby -e'puts Gem.default_dir')"
  gem install --ignore-dependencies --no-user-install -i "$pkgdir$_gemdir" -n "$pkgdir/usr/bin" $_gemname-$pkgver.gem
}
