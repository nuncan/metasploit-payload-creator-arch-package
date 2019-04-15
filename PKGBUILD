# Moved to AUR: GI_Jack <All American Zero>
# Updated: nuncan@github
# Original: ArchStrike <team@archstrike.org>
# Poached from Arch Strike

buildarch=1

pkgname=metasploit-payload-creator
pkgver=1.4.5
pkgrel=1
arch=('any')
pkgdesc="A wrapper to generate multiple types of payloads, based on users choice."
url="https://github.com/g0tmi1k/msfpc"
license=('MIT')
depends=('bash' 'metasploit')
provides=('mpc-git')
replaces=('mpc-git')
conflicts=('mpc-git')
source=("https://github.com/g0tmi1k/msfpc/archive/v${pkgver}.tar.gz")
sha512sums=('SKIP')

package() {
  cd msfpc-$pkgver
  install -dm755 "$pkgdir/usr/bin"
  install -dm755 "$pkgdir/usr/share/licenses/$pkgname"
  install -Dm644 LICENSE "$pkgdir/usr/share/licenses/$pkgname"
  install -Dm755 msfpc.sh "$pkgdir/usr/bin/msfpc.sh"
}
