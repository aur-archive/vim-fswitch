# Maintainer: Chris Sakalis <chrissakalis at gmail.com>
pkgname=vim-fswitch
pkgver=0.9.3
_scriptid=14047
pkgrel=1
pkgdesc='This script is designed to switch between companion files much like vimscript n.31 (a.vim).'
arch=("any")
url="http://www.vim.org/scripts/script.php?script_id=2590"
license=('custom:vim')
depends=('vim')
groups=('vim-plugins')
install=vimdoc.install
source=(${pkgname}-${pkgbuild}.zip::http://www.vim.org/scripts/download_script.php?src_id=${_scriptid}
        license.txt)

md5sums=('07805d341e39a9b55056be3d4640b1a2'
         '9d3d8bdd4b1719b8e5b13c4aef4e2a6c')
sha256sums=('e9e4317d9ae78a34d4e2e3c77704992154433b9fe81db7a26518f3603668e308'
            '5db4a4ea7b87af98253d1c1c783ea35b0b5a570c4f9cf759db00d0135d4bd7ad')

package() {
    install -d ${pkgdir}/usr/share/vim/vimfiles/{doc,plugin}
    install -Dm644 ${srcdir}/${pkgname}/doc/fswitch.txt ${pkgdir}/usr/share/vim/vimfiles/doc/fswitch.txt
    install -Dm644 ${srcdir}/${pkgname}/plugin/fswitch.vim ${pkgdir}/usr/share/vim/vimfiles/plugin/fswitch.vim
    install -Dm644 ${srcdir}/license.txt ${pkgdir}/usr/share/licenses/${pkgname}/license.txt
}

