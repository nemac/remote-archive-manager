A simple Perl script for maintaining a local archive of backup files
being generated on a remote system.

This script uses rsync to create a local mirror of a remote directory
containing backup files.  The local mirror exactly mirrors the contents
of the remote directory.

It also populates a local archive of copies of the files from the
local mirror.  The files in the archive are deleted based on their
age, regardless of when or if they disappear from the remote system.
