# Maintainer: zayronxio <https://github.com/sh4nks/pkgbuilds>
# Author: zayronxio
pkgname=cratos-lion-theme 
_pkgname=cratos-lion-theme
pkgver=3.0
pkgrel=2
pkgdesc="theme for xfce4, that mimics the look of Apple OS X."
arch=('i686' 'x86_64')
url="http://zayronxio.blogspot.mx/2012/02/cratoslion-tema-estilo-mac-para-gnome-y.html"
license=('GPL2')
depends=('gtk-engine-murrine' 'gtk2-xfce-engine' 'cratos-lion-icons' 'ttf-source-sans-pro' 'otf-texgyre' 'ttf-mac-fonts')
source=(https://dl.dropbox.com/u/64881799/Cratos-lion-theme.tar.gz)
md5sums=('655b0c0b0d0f0d7669d420f90a995bfc')

package() {
	mkdir -p ${pkgdir}/usr/share/themes/
    for T in *tar.gz
            do
                local FOLDER=`basename $T .tar.gz`
                mkdir $FOLDER
                bsdtar -zxf $T -C $FOLDER
            done

    cp -r */ ${pkgdir}/usr/share/themes/
}

