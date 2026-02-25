Ant Linux is a "Linux Distro" I made for RAM only stateless networking terminal laptops - mostly that surplus Chromebook I had access to. It's not just a toy - it's meant to be useful.
But I just wish to show that I do in fact have Linux experience and ability to produce novel Linux setups.

This system is designed for firewalling and routing with ufw to ensure control over slave units (stop them from phoning home without permission for example).
It has Librewolf for web browsing with builtin uBlock Origin, and MPV/yt-dlp for watching URLs with low resource footprint. Sway is included for GUI multiplexing.
And mostly the primary tool is foot and dbclient for actual control and data transfer between the slave units - wpa_supplicant is used to create a AP/hotspot and a STA device on the same phy for example.

The concept is as simple as above really. A very basic init system is used as a result. The whole point is that this role does not need to have persistence to work well.
So it runs purely in RAM. It expects as a result - a monolithic kernel with needed drivers baked in (not modules) and even better a DTB with NOR (SPI) and storage disabled.
