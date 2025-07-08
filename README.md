# busybox Doc 2025
![License](https://img.shields.io/badge/license-GPLv2-blue.svg)
![Repo Size](https://img.shields.io/github/repo-size/SahrulGunawan-ID/busybox)
![Last Commit](https://img.shields.io/github/last-commit/SahrulGunawan-ID/busybox)
![Stars](https://img.shields.io/github/stars/SahrulGunawan-ID/busybox?style=social)

#Old Version 
Version busybox-1.29.0

#Up To The Latest Version
busybox-1.37.0

# Comparison 
Old and New Versions Have Bugs If You Use Latest Version of GCC Old Version and Even New Version 1.37.0 If Gcc Version 12-15 . Stable Version For GCC 11.4.0

# How to Upgrade 
This Is The Latest Version For The Old Version Of Path Same : busybox-1.37.0/scripts/kconfig/lxdialog/check-lxdialog.sh

# Old Version Or New Version
# TO GCC 9-11
````bash
check() {
        $cc -x c - -o $tmp 2>/dev/null <<'EOF'
#include CURSES_LOC
main() {}
EOF
````

# Fix Use This Script 
# GCC 11 TO 15 Support
#If You Are Using GCC Version 12 Or Higher 15
````bash
check() {
    $cc -x c - -o $tmp 2>/dev/null <<'EOF'
#include CURSES_LOC
int main() { return 0; }
EOF
````

Old Versions of GCC Only Support Some If You Don't Change You Will Get Error Messages In the
```` error
EOF
	if [ $? != 0 ]; then
	    echo " *** Unable to find the ncurses libraries or the"       1>&2
	    echo " *** required header files."                            1>&2
	    echo " *** 'make menuconfig' requires the ncurses libraries." 1>&2
	    echo " *** "                                                  1>&2
	    echo " *** Install ncurses (ncurses-devel) and try again."    1>&2
	    echo " *** "                                                  1>&2
	    exit 1
````
This Error Is Located In

busybox-1.37.0/scripts/kconfig/lxdialog/check-lxdialog.sh

Thank you to all of you 
Pub Website : https://busybox.net
<br>Git Post : https://github.com/SahrulGunawan-ID/busybox
