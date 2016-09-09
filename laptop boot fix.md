Laptop sent off for repair 5/15/2016.  SSD w/ Win7/Linux Mint dual-boot removed and original SSHD replaced in laptop, no boot settings were modified.
Laptop picked up 6/13/2016 with “Windows Boot Manager has been blocked by current security policy” message present when SSD was replaced in machine.
Steps to fix:
Enter into BIOS
Boot → Secure Boot → Disable
Boot → UEFI Boot → Use F5/F6 to move “Ubuntu” and “Windows Boot Manager” to the first two options above the NIC boot.
Exit → Exit saving changes
Anddd...voila.

