To overcome <br><i><b>make[2]: *** [scripts/Makefile.build:268: /var/lib/dkms/rtl8723de/5.1.1.8_21285.20171026_COEX20170111-1414/build/os_dep/linux/rtw_proc.o] Error 1 make[1]: *** [Makefile:1683: /var/lib/dkms/rtl8723de/5.1.1.8_21285.20171026_COEX20170111-1414/build] Error 2</b></i> 
<i><b>! </b> use at your own risk</i> since not tested on multiple devices
! Worked for me. Tested on manjaro/Arch linux5.6 kernel.
# rtl8723de
Realtek RTL8723DE module for Linux kernel version 5

Install:

    git clone https://github.com/Dhirajraje/rtl8723de.git -b current
    dkms add ./rtl8723de
    dkms install rtl8723de/5.1.1.8_21285.20171026_COEX20170111-1414
    depmod -a
    reboot

Uninstall:

    check main source @ https://github.com/smlinux/rtl8723de
