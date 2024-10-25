# eplug (README UNDER CONSTRUCTION)
## Intro
eplug is a plug manager for portage that allows you to make portage do what you want it to a little bit easier!

This project is still heavily work-in-progress and a ebuild for this should soon be available in basil-overlay!

## Usage
For now - To install eplug you just place the files in [portage](./portage) into `/etc/portage/`

Then uncomment/add lines in `/etc/portage/plugins.load` to enable plugins from `/etc/portage/plugins/`

## Legacy Notes
If you want to continue to use the original ehook instead of migrating to the eplug version then you are safe to continue using the v1.1 tag

If you want to migrate from the original ehook to the eplug port of legacy ehook then you can just install eplug normally, rename package.ehook to hook, and uncomment the `legacy/ehook` line in /etc/portage/plugins.load

If you'd like to migrate to the modern ehook plugin (v1.2+) then you can use the configuration in [config-examples](./config-examples/plugin_ehook) for an example of a simple grub mkconfig hook on kernel updates

For anything else there will be more documentation in the near future that will explain eplug in more depth
