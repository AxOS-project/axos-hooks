# Maintainer: Ardox

pkgname="axos-hooks"
pkgver=3.12
pkgrel=1
pkgdesc='Hooks for AxOS filesystem'
arch=('x86_64')
license=('GPL3')
source=(
		'axos-hooks.hook'
		'axos-os-release.hook'
		'axos-lsb-release.hook'
		'axos-sleex-skel.hook'
		'axos-reboot-required.hook'
		'axos-plymouth.hook'
		'axos-hooks-runner'
		'axos-reboot-required'
		'axos.png'
		'axos.svg'
		'axos-logo.png'
		'axos-logo.svg'
		'axos-full-update'
)

sha256sums=('b375a7b3669cc3807ee8ce1f3db52de0421bf58d0cc1af2db2ad549abe54f20b'
            'd5a418811752d03bdd84eb55204abfe55ed32da5ea2c523ec90fab5c2f8447fe'
            'cafa8c21eb2c4619d623d9edd596c7feb23c8f30323b505dc88dc7954f96fc3f'
            'f69a309cc0243d4e8aab8b1bdaa23a6aeeaf2958ff060047f1d34ccdce697f20'
            'a47d75cf4d422bd8780aac566bb6fc7a827f2af3ecd8bfdbab5804d73b895a02'
            '7db2cc384826ce2fc90bbfee526157561e04991cdcb9ac8e789037db1719141b'
            '29d8cd2f85d7116394378b90e9b612de2b64f6354f03cd829d5f2ec9dd3eda77'
            'c069eacd2fb09b6d648dea897bc4de4f8f26c9cf04ddfdd5d39019b13eafcd21'
            '22f2eff360ef6f68f9af2ae709345299a147233123a7f90d34e1e03e29bef628'
            '81eecdabee81aa907275a1faa95e41c704eefab9059a8a522775378d125760dd'
            '933eb942ed6e266f93243463a6a1cc811d9c5ccdc48fa89847fe775961a99279'
            '81eecdabee81aa907275a1faa95e41c704eefab9059a8a522775378d125760dd'
            'f74f9102b653032524bf16f48b4d5fb89303ed3f2b5871f26b597bf59fdcab5d')
			
package() {
	local hooks="$pkgdir"/usr/share/libalpm/hooks
	local pixmaps="$pkgdir"/usr/share/pixmaps
	local bin="$pkgdir"/usr/bin

	install -Dm 644 axos-hooks.hook           	"$hooks"/axos-hooks.hook
	install -Dm 644 axos-lsb-release.hook      "$hooks"/axos-lsb-release.hook
	install -Dm 644 axos-os-release.hook       "$hooks"/axos-os-release.hook
	install -Dm 644 axos-reboot-required.hook  "$hooks"/axos-reboot-required.hook
	install -Dm 664 axos-plymouth.hook         "$hooks"/axos-plymouth.hook
	install -Dm 664 axos-sleex-skel.hook         "$hooks"/axos-sleex-skel.hook

	install -Dm 755 axos-hooks-runner         	"$bin"/axos-hooks-runner
	install -Dm 755 axos-reboot-required       "$bin"/axos-reboot-required
	install -Dm 755 axos-full-update 			"$bin"/axos-full-update

	install -Dm 644 axos.png       			"$pixmaps"/axos.png
	install -Dm 644 axos.svg       			"$pixmaps"/axos.svg
	install -Dm 644 axos-logo.png       		"$pixmaps"/axos-logo.png
	install -Dm 644 axos-logo.svg       		"$pixmaps"/axos-logo.svg
}
