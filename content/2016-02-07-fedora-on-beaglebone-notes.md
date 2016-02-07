Title: Fedora on BeagleBone Black  
Date: 2016-02-07 14:05
Modified: 2016-02-07 14:05
Category: short tips
Slug: fedora-on-beaglebone-black
Authors: Jon Moore

Following the [Fedora ARM Installation Guide](https://fedoraproject.org/wiki/Architectures/ARM/F23/Installation) makes getting the Fedora ARM image running on the BeagleBone fairly easy.  This is my notes on some extra or not easily documented changes I had to make.

1. If using the Minimal image and you do not have a serial console it is best to use the fedora-arm-installer and set no root password.

2. After getting the image installed us `parted resizepart` and `resize2fs` to grow the root filesystem.

3. After resizing I did follow the steps on the Wiki to install U-Boot to media.  I do not know if this is done by the fedora-arm-installer scripts or not.  
