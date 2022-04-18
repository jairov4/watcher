# Watcher

Generic wrapper that monitors the filesystem and restart a program on change.

Inspired in https://github.com/radovskyb/watcher

# Usage

```text
> watcher -h

Usage of ./watcher:
  -cmd string
        command to run when an event occurs
  -dotfiles
        watch dot files (default true)
  -ignore string
        comma separated list of paths to ignore
  -interval string
        watcher poll interval (default "100ms")
  -list
        list watched files on start
  -recursive
        watch folders recursively (default true)
```

Example

```bash
# Watch the current folder and all its files and restart the server on change
watcher -cmd "python serve.py"
```
