# xcat-syncfilez
Lightweight drop-in replacement for the xcat syncfiles postscript

## Compatibility

This is intended for modern Linux distributions, and drops all of the legacy compatibility code in the original xcat code.
```
# cat syncfiles startsyncfiles startsyncfiles.awk startsyncfiles.aix | wc -l
237
# cat syncfilez | wc -l
33
```

## Installation

Copy the script to `/install/postscripts` on the head node.

You can either replace `syncfiles` in the postscripts tab by using `tabedit postscripts` or add it to the osimage definition's `postscript` or `postbootscript` fields.

