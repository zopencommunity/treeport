tree

The tree command is a very usefull utility that will display directories and files in a tree like structure.
This version has been enhanced to support z/OS specific functions:
- The protection bits with option `-p` will show a `+` to the right if an ACL is present
The following options are formatted according to the output of the `ls -lET` command.
- The `--extended` option will show the extended attributes with the protection bits. Specifying `--extended` enables `-p` by default.
- The `--filetag` option will show filetag information for the files.
- The `-z` option is a convenience option to enable all z/OS specific information at once.

Example command that will show all files in the users home dir and will also color according to the LS_COLORS environment variable.

It will format the tree nicely using utf8 tree characters if the terminal supports it.

`tree -zC --charset=uft8 ~`
