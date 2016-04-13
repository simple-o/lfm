# Introduction #

Last File Manager is a powerful file manager for the UNIX console.
It has a curses interface and it's written in Python.

Some of the features you can find in lfm:

  * console-based file manager for UNIX platforms
  * 1-pane or 2-pane view
  * bookmarks
  * history
  * vfs for compressed files
  * dialogs with entry completion
  * PowerCLI, a command line interface with advanced features
  * fast access to the shell
  * direct integration of find/grep, df and other tools
  * tabs
  * color files by extension
  * fast file viewer with text and binary modes
  * ...and many others


# Screenshots #

**lfm**:

![http://www.terra.es/personal7/inigoserna/lfm/lfm.png](http://www.terra.es/personal7/inigoserna/lfm/lfm.png)

**pyview**:

![http://www.terra.es/personal7/inigoserna/lfm/pyview.png](http://www.terra.es/personal7/inigoserna/lfm/pyview.png)


# Requirements #

Lfm and Pyview are written in Python and require curses module. It needs Python v2.5 or higher, it won't work with older versions.

Since version 0.90, lfm needs ncurses >= v5.x to handle terminal resizing.

Python v2.5+ and ncurses v5.4+ to use wide characters.

Note that python curses module should be linked against ncursesw library (instead of ncurses) to get wide characters support. This is the usual case in later versions of Linux distributions, but maybe not the case in older Linux or other UNIX platforms. Thus, expect problems when using multibyte file names (f.e. UTF-8 or latin-1 encoded) if your curses module isn't compiled against ncursesw. Anyway, I hope this issue will disappear with new releases of those platforms eventually.

Consult Files name encoding section below for more information about support of different encodings.

All modern UNIX flavours (Linux, BSD, Solaris, etc) should run it without problems. If they appear please notify me.

Finally, take a look at TODO file to see bugs and not-implemented-yet (tm) features.