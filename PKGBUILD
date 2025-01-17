# Maintainer: Jakub Kopańko <hi at kopanko dot com>

pkgname=hcp-bin
pkgver=0.8.0
pkgrel=1
pkgdesc="Lets you administer HashiCorp Cloud Platform (HCP) resources and services."
arch=('x86_64' 'aarch64')
url="https://github.com/hashicorp/hcp"
license=("MPL-2.0")
provides=("hcp=${pkgver}")
conflicts=('hcp')

source_x86_64=("https://releases.hashicorp.com/hcp/${pkgver}/hcp_${pkgver}_linux_amd64.zip")
sha256sums_x86_64=('5b00869908c25ff68291b51c5d3538655eb31b927c71db37baa7b89441e99f78')

source_aarch64=("https://releases.hashicorp.com/hcp/${pkgver}/hcp_${pkgver}_linux_arm64.zip")
sha256sums_aarch64=('b98b0a535263b0947aee13e8abdc5d1f402b316d5535201c6903abe96335fb09')

package() {
    install -Dm755 "${srcdir}/hcp" "${pkgdir}/usr/bin/hcp"
}
