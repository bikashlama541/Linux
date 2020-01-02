# Steps by steps instruction to change PW of root in RHEL.

1) while booting  press e 
2) UTF -0 rd.break
3) Press ctrl X
4)mount -o remount,rw /sysroot
5)chroot /sysroot
6)passwd ... again ......

7)touch /.autorelabel 

8)exit

9)exit
