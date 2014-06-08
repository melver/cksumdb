=======
cksumdb
=======

Simple BASH script to generate file checksums in various database formats.

At the moment the follow backends are provided:

file: Store metadata in an identical tree.

xattr: Store metadata in extended attributes, if supported by filesystem (e.g.
ext4).

Unlike xattr, the file backend still works if files only have read permissions,
but not write permissions.

Alternatives
------------

Alternatives, that accomplish similar goals:

https://github.com/rfjakob/cshatag
https://bitbucket.org/maugier/shatag
Both are similar, in that they store the checksum in file's file's extended
attributes. cksumdb can support EAs as another DB-backend.

https://github.com/BlackIkeEagle/par2cmdline
Can do error recovery, but is much slower.

http://en.wikipedia.org/wiki/ZFS
This would be the preferred choice -- if we can use ZFS -- for the purpose I
wrote cksumdb for.
