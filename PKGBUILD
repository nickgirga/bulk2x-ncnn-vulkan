# Maintainer: Nicholas Girga <contact@nickgirga.com>
pkgname='bulk2x-ncnn-vulkan'
pkgver=r18.e057a4d
pkgrel=1
pkgdesc="Simple GUI to make it easy to use waifu2x-ncnn-vulkan"
arch=('any')
url="https://gitlab.com/nickgirga/bulk2x-ncnn-vulkan"
license=('GPL3')
depends=('python' 'python-gobject' 'gtk3' 'waifu2x-ncnn-vulkan-git')
source=('bulk2x-ncnn-vulkan-git::git+https://gitlab.com/nickgirga/bulk2x-ncnn-vulkan.git')
md5sums=('SKIP')

pkgver() {
	cd "$srcdir/bulk2x-ncnn-vulkan-git"
	printf "r%s.%s" "$(git rev-list --count HEAD)" "$(git rev-parse --short HEAD)"
}

package() {
    cd "$srcdir/bulk2x-ncnn-vulkan-git"
    install -Dm755 ./bulk2x-ncnn-vulkan "$pkgdir/usr/bin/bulk2x-ncnn-vulkan"
    install -Dm644 ./main.glade "$pkgdir/usr/share/bulk2x-ncnn-vulkan/main.glade"
    install -Dm644 ./res/icon.svg "$pkgdir/usr/share/bulk2x-ncnn-vulkan/res/icon.svg"
    install -Dm644 ./bulk2x-ncnn-vulkan.desktop "$pkgdir/usr/share/applications/bulk2x-ncnn-vulkan.desktop"
}
