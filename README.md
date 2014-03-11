vmware_patch
============

original patch where found on:

for vmnet
* http://rglinuxtech.com/?p=1008
* http://pastebin.com/p3bkbAMu

for vmblock
* http://mysticalzero.blogspot.com.au/2013/07/vmblock-patch-for-linux-310-vmware.html
* http://mysticalzero.blogspot.co.uk/2013/07/vmblock-patch-for-linux-311-rc1-vmware.html
* http://dominator008.com/constructionyard/2013/10/03/vmware-9-0-2-vmblock-patch-for-linux-kernel-3-12/

How apply them

vmnet:
* $ tar -xvf /usr/lib/vmware/modules/source/vmnet.tar
* $ patch -p1 < vmnet-patch-kernel-3.13
* $ tar -uf vmnet.tar vmnet-only
* # cp vmnet.tar /usr/lib/vmware/modules/source/
 
vmblock:
* $ tar -xf /usr/lib/vmware/modules/source/vmblock.tar
* $ patch -p1 < vmblock-patch-kernel-3.13
* $ tar -uf vmblock.tar vmblock-only
* # cp vmblock.tar /usr/lib/vmware/modules/source/
