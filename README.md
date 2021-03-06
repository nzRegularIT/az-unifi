# az-unifi

## References

## VM Deploy and UniFi Install
* https://help.ui.com/hc/en-us/articles/220066768-UniFi-Network-How-to-Install-and-Update-via-APT-on-Debian-or-Ubuntu
* https://help.ui.com/hc/en-us/articles/218506997-UniFi-Ports-Used
* https://gist.github.com/davecoutts/5ccb403c3d90fcf9c8c4b1ea7616948d
* https://docs.microsoft.com/en-us/azure/virtual-machines/linux/tutorial-automate-vm-deployment
* https://cloudinit.readthedocs.io/en/latest/topics/examples.html
* https://www.kenmuse.com/blog/arm-templates-and-cloud-init
* https://docs.microsoft.com/en-us/azure/virtual-machines/linux/cloud-init-deep-dive
* https://docs.microsoft.com/en-us/azure/virtual-machines/linux/cloud-init-troubleshooting#step-4-investigate-why-the-configuration-isnt-being-applied
* https://help.ui.com/hc/en-us/articles/204952144#4
* https://help.ui.com/hc/en-us/articles/215458888-UniFi-USG-Advanced-Configuration-Using-config-gateway-json

### Automatic Updates
* https://community.ui.com/questions/unifi-apt-get-upgrade-prompt-for-backups/f2ac7635-07f4-46fe-aeda-2933af474174
* https://libre-software.net/ubuntu-automatic-updates/
* http://blog.ezyang.com/2010/03/third-party-unattended-upgrade/
* http://dl-origin.ubnt.com/unifi/debian/dists/stable/Release
* https://askubuntu.com/questions/87849/how-to-enable-silent-automatic-updates-for-any-repository

### Automatic Updates Config Files
`````
sudo cat /etc/apt/apt.conf.d/20auto-upgrades | gzip | base64 -w0
sudo cat /etc/apt/apt.conf.d/50unattended-upgrades | gzip | base64 -w0
`````