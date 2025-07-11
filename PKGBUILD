# Maintainer: Ardox

pkgname="axos-hooks"
pkgver=3.15
pkgrel=2
pkgdesc='Hooks for AxOS filesystem'
arch=('x86_64')
license=('GPL3')
source=(
		'axos-release.hook'
		'axos-sleex-skel.hook'
		'axos-reboot-required.hook'
		'axos-plymouth.hook'
		'axos-hooks-runner'
		'axos-reboot-required'
		'axos.png'
		'axos.svg'
		'axos-logo.png'
		'axos-logo.svg'
)

sha256sums=('83e015ff0d43b7aed4b53cf1df235aa6d2d9d419bdc7b73bebd377a76836e9c6'
            '14ee99fb24a0022cb39eb8b3ead2c0cc676f39b973701b75b15ea3fe8aee8ed6'
            'a47d75cf4d422bd8780aac566bb6fc7a827f2af3ecd8bfdbab5804d73b895a02'
            '7db2cc384826ce2fc90bbfee526157561e04991cdcb9ac8e789037db1719141b'
            'b009f2445b7a1a23d0e573f87e6d61999c95005da423b25cdbc808277dacdc73'
            'c069eacd2fb09b6d648dea897bc4de4f8f26c9cf04ddfdd5d39019b13eafcd21'
            '22f2eff360ef6f68f9af2ae709345299a147233123a7f90d34e1e03e29bef628'
            '81eecdabee81aa907275a1faa95e41c704eefab9059a8a522775378d125760dd'
            '933eb942ed6e266f93243463a6a1cc811d9c5ccdc48fa89847fe775961a99279'
            '81eecdabee81aa907275a1faa95e41c704eefab9059a8a522775378d125760dd')

package() {
	local hooks="$pkgdir"/usr/share/libalpm/hooks
	local pixmaps="$pkgdir"/usr/share/pixmaps
	local bin="$pkgdir"/usr/bin

	install -Dm 644 axos-release.hook      "$hooks"/axos-release.hook
	install -Dm 644 axos-reboot-required.hook  "$hooks"/axos-reboot-required.hook
	install -Dm 664 axos-plymouth.hook         "$hooks"/axos-plymouth.hook
	install -Dm 664 axos-sleex-skel.hook         "$hooks"/axos-sleex-skel.hook

	install -Dm 755 axos-hooks-runner         	"$bin"/axos-hooks-runner
	install -Dm 755 axos-reboot-required       "$bin"/axos-reboot-required

	install -Dm 644 axos.png       			"$pixmaps"/axos.png
	install -Dm 644 axos.svg       			"$pixmaps"/axos.svg
	install -Dm 644 axos-logo.png       		"$pixmaps"/axos-logo.png
	install -Dm 644 axos-logo.svg       		"$pixmaps"/axos-logo.svg
}
