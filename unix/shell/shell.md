# [Unix Shell](http://www.wikiwand.com/en/Unix_shell)
## Variables
All active variables can be seen by running `env`.
- `$HOME` - Expands to the path of my home folder.
- `$PS1` - Variable that represents my command prompt line.
- `$PATH` - Special environment variable that contains the command path (list of system directories that the shell searches when trying to locate a command).

## Notes
- Scripts are run in subshells, and nothing is shared "upwards". That's the difference between running a script and sourcing one. A sourced (imported) script is run in your own script's namespace.
- In shell everything is a string.
- Children never touch parent enviroment. It can only if it runs as part of the current process (source, function, alias).
- Pipes are used to connect one process's output with another process’s input.

## Links
- [Explain Shell](https://www.explainshell.com/)
- [Introduction to POSIX Shell](http://sircmpwn.github.io/2018/02/05/Introduction-to-POSIX-shell.html)
- [Yoshua's notes](https://yoshuawuyts.gitbooks.io/knowledge/content/unix/shell.html)
- [Shell Auto-completion Systems](http://dundalek.com/entropic/shell-auto-completion/)

## Snippets
- [Standard input & output](https://gist.github.com/a1346899be8f2e186e161f1a03efd52b)
- [Globbing](https://gist.github.com/7d9564e24242cda9c0a6717021971830)