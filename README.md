# Automating a nested VMware ESXi install with Powercli

...
Date: 30-9-2019
...

...
Version: 1
...

...
Blog: www.sysadmintutorials.com
...

...
Twitter: @systutorials
...

## Description

This PowerCLI script will allow you to perform the installation of a nested VMware ESXi host, have the VM reboot and then perform the configuration of the host.

## Important Notes
  
  * Make sure you have PowerCLI installed, if you are not sure how to install PowerCLI see this blog post:
  https://thesolving.com/virtualization/how-to-install-and-configure-vmware-powercli-version-10/
  * This script works with VMware ESXi 6.5 and beyond
  * Change the vcenter variable to match your vcenter server IP or DNS name:
  $VcenterServer = "vmvcenter.vmlab.local" #Vcenter Server that contains the nested esxi host - Replace with your vCenter server address
  * Set the configuration you would like to use under the '# Set your Variables here'
  If you will be using a VLAN, set $UseVlan = "Yes" and then enter in the $VlanID
  * To see a demo of the script please checkout my youtube video: https://youtu.be/Q2muTWjAmgY
