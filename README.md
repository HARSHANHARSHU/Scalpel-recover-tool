# Scalpel-recover-tool
scalpel is a fast file carver that reads a database of header and footer definitions and extracts matching files from a set of image files or raw device files.

scalpel is filesystem-independent and will carve files from FAT16, FAT32, exFAT, NTFS, Ext2, Ext3, Ext4, JFS, XFS, ReiserFS, raw partitions, etc.

scalpel is a complete rewrite of the Foremost 0.69 file carver and is useful for both digital forensics investigations and file recovery.


_________________________________________________________________________________________________________________________
Installed size: 88 KB
How to install: sudo apt install scalpel
_________________________________________________________________________________________________________________________
commands
apt-get install scalpel
man scalpel 
vi /etc/scalpel/scalpel.conf
[...]
        pdf     y       5000000 %PDF  %EOF\x0d  REVERSE
        pdf     y       5000000 %PDF  %EOF\x0a  REVERSE
[...]
scalpel /dev/sda1 -o <filename> 
mount
ls -la
ls -l <filename>
cat <filename>/audit.txt
ls -l <filename>/pdf-0-0/
