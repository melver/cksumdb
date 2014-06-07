=======
cksumdb
=======

Simple BASH script to generate file checksums in various database formats.

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
