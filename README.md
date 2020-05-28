# exim4-privesc
*Credit to Tib3rius* | https://tryhackme.com/room/linuxprivesc

Find all the SUID/SGID executables on the Debian VM:

find / -type f -a \( -perm -u+s -o -perm -g+s \) -exec ls -l {} \; 2> /dev/null

If /usr/sbin/exim-4.84-3 appears in the results, use cve-2016-1531.sh to gain a root shell.

[![Image of suid](https://github.com/kam1n0/exim4-privesc/blob/master/tmp_upload/suid.png)(#)]

link root
