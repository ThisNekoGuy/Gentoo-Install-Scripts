# Gentoo-Install-Scripts
An install script to automate setting up a base gentoo system. Note: An ncurses based ui, or a toolkit based GUI <em>may</em> be coming. Depends on contributions.

# Usage
Download a stage3 tarball from gentoo's website, and place it in the stage3 folder. Boot the gentoo live cd, and clone this repository in the live cd. Then create your partitions, and run the script. 

# Important 
By default the script uses the default partition table in the gentoo handbook

Filesystem<br />
`/dev/nvme0np3 ->` Boot partition<br />
`/dev/nvme0np3 ->` Swap partition<br />
`/dev/nvme0np3 ->` Root partition<br />
-or-
`/dev/sda1 ->` Boot partition<br />
`/dev/sda2 ->` Swap partition<br />
`/dev/sda3 ->` Root partition<br />
 
This script will need some modifications especially the kernel config file. These modifications depend on your system. Also this script uses openrc as its primary init system. Also the script at this point in time doesn't automatically download a stage3 tarball you will have to do that your self and place it in the stage3 folder.

Another thing to note is that the script by default builds for UEFI systems. This can easily be changed

