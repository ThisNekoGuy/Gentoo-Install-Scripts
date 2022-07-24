# Gentoo-Install-Scripts
An install script to automate setting up a base gentoo system. Note: An ncurses based UI, or a toolkit based GUI <em>may</em> be coming. Depends on contributions.

# GitLab Page
https://gitlab.com/N3k0-san/Gentoo-Install-Scripts

# GitHub Mirror
https://github.com/ThisNekoGuy/Gentoo-Install-Scripts

# Usage
Boot the Gentoo live cd and clone this repository inside the live cd. Then, create your partitions and run the script.

# Important 
By default, the script does not use the partition table in the Gentoo handbook.
Be sure to partition your drive first, and check the script to make sure it targets the correct drive near the top (simple to do); no need to format it, the script does this.

Filesystem<br />
`/dev/nvme0np1 ->` Boot partition<br />
`/dev/nvme0np2 ->` Swap partition<br />
`/dev/nvme0np3 ->` Root partition<br /><br />
-or-<br /><br />
`/dev/sda1 ->` Boot partition<br />
`/dev/sda2 ->` Swap partition<br />
`/dev/sda3 ->` Root partition<br />
 
This script will need some minor modifications; especially for the kernel config file (either you will need to supply your own or use the default <em>"USE_KERNEL_CONFIG=false"</em> value). These modifications depend on your system. Also, this script uses OpenRC as its primary init system.

At the moment, the script installs KDE Plasma and the proprietary Nvidia driver by default (the GPU driver can be changed).

Another thing to note is that the script by default builds for UEFI systems. This can be changed.

# Original Upstream URL:
https://github.com/tashrifsanil/Gentoo-Install-Scripts

