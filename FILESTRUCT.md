#This file contains the file structure used.
--- 

### Tools structure
All the packages and tools will be added in config/package-lists/
and there are different file with extension .list.chroot used for this purpose ... Desktop is for environent and ui tool.
anon is for security ,privacy and stealth tools.
pentest for pentesting and hacking tools.
devtools for development tools and langs.

### Hooks or default tools
All the default tool will go in config/hook/normal with .hook.chroot extension.
Along with tor routing , macchanger and kill switch .

## Main folders with their tasks are mention below

core(main home folder for running build)
config(main config folder for entire build , present insde core folder)
|->hooks(all the tasks that need to run by default at different stages need to go here with extension .hook.chroot or .hook.binary acording to their initiation stages)
|    |->live(not to be modified)
|    |->normal(all files for default intiation at either boot or startup go here)
|->includes.binary/boot/grub(configs and theme for GRUB go here)
|->includes.chroot_after_packages/share(all the images , icons ,etc to be shared via across the os)
|->package-lists(list of all the packages that need to be installed)
     |->anon(for privacy concerning tools like tor and macchanger)
     |->desktop(tools for desktop environement)
     |->devtool(for tools and langs for development and programming)
     |->pentest(for all pentesting tool)
|->packages(any package .deb to be added locally build){curretly missing due to lack of any local .deb package}
|->other config files 
