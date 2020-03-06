# `resymbolicate`

A simple script that symbolicate crash logs on the command-line, given a list of paths containing symbols.

Basic usage is:
```bash
symbolicate <crash log> <symbol 1> <symbol 2> ...
```

Example usage:
```bash
symbolicate foo/crash.log bar.app/Contents/macOS/bar
```

> The script **will overwrite** the existing crash log.
