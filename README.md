# `symbolicate`

A simple script that symbolicate crash logs on the command-line, given a list of paths containing symbols.

Basic usage is:
```bash
symbolicate <crash log> <path 1> <path 2> ...
```

Example usages:
```bash
symbolicate foo/crash.log bar.app/Contents/macOS/bar
symbolicate foo/crash.log bar.app.DSYM/bar.app.dSYM/Contents/Resources/DWARF/bar
symbolicate foo/crash.log bar.app.DSYM/**/DWARF/* # Only supported in certain shells (tested on zsh)
```

> The script **will overwrite** the existing crash log.
