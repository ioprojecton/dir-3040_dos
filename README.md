# dir-3040 Denial of Service
Dir-3060 might also be affected as they share many components from same firmware.

Tested on latest firmware 1.20b03a hotfix

ftp server user access page by default is configured for any user with write privileges to write directly to ram instead of restricting to usb drives only.

There are no out of bound or buffer overflow checks in place in latest firmware for this issue.

After writing(filling) available memory system will crash and reboot.

User doesnt need to have administrator privileges to perform the attack.

proof of concept in detail with pictures below

D-link was contacted and strongly denied presence of the issue because they couldnt reproduce the issue.

