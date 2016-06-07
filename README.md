# svn2git

Patch replayer, that migrates a Subversion repository to a local Git working
copy.

## help

```
Converts a Subversion repository into a local Git working copy via patch replay
syntax: svn2git SVN GIT [SVN-START SVN-END]

        SVN         URL describes Subversion repository
        GIT         Path to directory, that hold's the new Git
                    working copy
        SVN-START   Subversion Revision to start
        SVN-END     Subversion Revision to end

svn2git, Copyright (C) 2016 Alexander Böhm <alxndr.boehm@gmail.com>
Licensed under GPLv2. See source distribution for detailed
copyright notices.
```

To activate status output, set the environment VERBOSE=1.

## example

Convert Subversion repository http://svn.gna.org/svn/maker into Git repository
under /tmp/maker from Revision 10 upto 20.

```
svn2git http://svn.gna.org/svn/maker /tmp/maker 10 20
```

