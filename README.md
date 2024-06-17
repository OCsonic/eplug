# ehook
## Usage
ehook allows for running bash scripts at the start of an ebuild phase for gentoo packages.

To use ehook you just create the following directory tree in your portage directory (the same folder where your make.conf is located.) "package.hook/category/package-name/ebuild_phase" then place scripts inside of it to run at the beginning of the given ebuild phase for that package.

example of a valid script placement:
`/etc/portage/package.hook/sys-kernel/gentoo-kernel/postinst/00-grub_regenerate_config`

## Installation
Place ehook and bashrc in your portage directory.