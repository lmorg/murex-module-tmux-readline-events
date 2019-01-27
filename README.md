# Murex module: tmux-readline-events

This _murex_ module provides the help and edit hotkeys:

## tmux-readline-event-help:

Press `{F1}` when you have a command line written and to trigger a help pane
with the man page on the command (or source code for functions) as well as a
cheat sheet on it's usage (if one exists).

## tmux-readline-event-edit:

Press `{CTRL+E}` when you have a partial command line written to bring up a
full screen editor (defined either via `export EDITOR` or `config set shell
editor`).

* If a filename exists in the path, then the editor would be for that file.

* If no file name exists, but the calling command is a _murex_ function, then
  the editor would be for that function.

## Other hotkeys already provided by `readline`:

If you enter `vi` mode (hit `{ESC}` on the command prompt) then press `v` to
start the "visual editor" (aka which ever editor is defined in `$EDITOR`.

The `config set shell editor` method will also change that value here too.
