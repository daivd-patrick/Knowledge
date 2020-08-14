# [Unix Shell](http://en.wikipedia.org/wiki/Unix_shell)

## Variables

All active variables can be seen by running `env`.

- `$HOME` - Expands to the path of my home folder.
- `$PS1` - Variable that represents my command prompt line.
- `$PATH` - Special environment variable that contains the command path (list of system directories that the shell searches when trying to locate a command).

## Notes

- Scripts are run in subshells, and nothing is shared "upwards". That's the difference between running a script and sourcing one. A sourced (imported) script is run in your own script's namespace.
- In shell everything is a string.
- Children never touch parent environment. It can only if it runs as part of the current process (source, function, alias).
- Pipes are used to connect one process's output with another process’s input.
- `/etc/paths.d` define paths to add to `$PATH` globally to all users.

## Links

- [Explain Shell](https://www.explainshell.com/)
- [Introduction to POSIX Shell](http://drewdevault.com/2018/02/05/Introduction-to-POSIX-shell.html)
- [Yoshua's notes](https://yoshuawuyts.gitbooks.io/knowledge/content/unix/shell.html)
- [Shell Auto-completion Systems](http://dundalek.com/entropic/shell-auto-completion/)
- [Shell and Scripting (2019)](https://hacker-tools.github.io/shell/)
- [ShellCheck](https://www.shellcheck.net) - Finds bugs in your shell scripts. [Code](https://github.com/koalaman/shellcheck).
- [Rash](https://github.com/willghatch/racket-rash) - The Reckless Racket Shell.
- [Eternal Terminal](https://github.com/MisterTea/EternalTerminal) - Remote shell that automatically reconnects without interrupting the session.
- [patat](https://github.com/jaspervdj/patat) - Terminal-based presentations using Pandoc.
- [What does your shell prompt look like? (2019)](https://lobste.rs/s/x5ioqm/what_does_your_shell_prompt_look_like)
- [direnv](https://direnv.net/) - Unclutter your .profile.
- [mask](https://github.com/jakedeichert/mask) - CLI task runner defined by a simple markdown file.
- [Purs](https://github.com/xcambar/purs) - Pure-inspired prompt in Rust.
- [Sampler](https://github.com/sqshq/sampler) - Tool for shell commands execution, visualization and alerting. Configured with a simple YAML file.
- [Nu Shell](https://github.com/nushell/nushell) - Modern, GitHub-era shell written in Rust. ([HN](https://news.ycombinator.com/item?id=20783006))
- [Collection of pure POSIX sh alternatives to external processes](https://github.com/dylanaraps/pure-sh-bible)
- [Lobsters: What does your shell prompt look like? (2019)](https://lobste.rs/s/skoapt/what_does_your_shell_prompt_look_like)
- [navi](https://github.com/denisidoro/navi) - Interactive cheatsheet tool for the command-line.
- [Announcing Alacritty, a GPU-accelerated terminal emulator](https://jwilm.io/blog/announcing-alacritty/)
- [What Is a Shell? (2019)](https://yunchi.dev/posts/what-is-a-shell/)
- [Lobsters: What shell do you use? (2019)](https://lobste.rs/s/tjjfnz/what_shell_do_you_use)
- [“Use Dumb Shell, don’t Reinvent the Wheel” (2020)](https://ilya-sher.org/2020/01/04/use-dumb-shell-dont-reinvent-the-wheel/) ([Lobsters](https://lobste.rs/s/b8xanw/use_dumb_shell_don_t_reinvent_wheel))
- [In search for a better job scheduler](https://beepb00p.xyz/scheduler.html) - What if cron and systemd had a baby? Wouldn't it be beautiful? ([HN](https://news.ycombinator.com/item?id=22087195))
- [Writing Safe Shell Scripts (2019)](https://sipb.mit.edu/doc/safe-shell/) ([HN](https://news.ycombinator.com/item?id=22212338))
- [Curl to shell isn’t so bad (2019)](https://www.arp242.net/curl-to-sh.html) ([HN](https://news.ycombinator.com/item?id=21490151))
- [Partial Tour Through the UNIX Shell](http://www.collyer.net/who/geoff/sh.tour.pdf)
- [ABS](https://github.com/abs-lang/abs) - Programming language that works best when you're scripting on your terminal.
- [Wez's Terminal](https://github.com/wez/wezterm) - GPU-accelerated cross-platform terminal emulator and multiplexer written in Rust.
- [Text processing in the shell (2020)](https://blog.balthazar-rouberol.com/text-processing-in-the-shell) ([HN](https://news.ycombinator.com/item?id=22590824))
- [Crush](https://github.com/liljencrantz/crush) - Attempt to make a command line shell that is also a powerful modern programming language.
- [nsh](https://github.com/nuta/nsh) - Command-line shell like fish, but POSIX compatible.
- [Three Comics For Understanding Unix Shell (2020)](http://www.oilshell.org/blog/2020/04/comics.html)
- [Oil Shell](http://www.oilshell.org/) - New Unix shell. ([Blog](http://www.oilshell.org/blog/))
- [asciinema](https://asciinema.org/) - Web player for terminal session recordings. ([Code](https://github.com/asciinema/asciinema-player))
- [svg-term-cli](https://github.com/marionebl/svg-term-cli) - Share terminal sessions via SVG and CSS.
- [Customizing your shell (2020)](https://blog.balthazar-rouberol.com/customizing-your-shell.html) ([HN](https://news.ycombinator.com/item?id=22898577))
- [tmate](https://tmate.io/) - Instant terminal sharing. ([Code](https://github.com/tmate-io/tmate))
- [Rich’s sh (POSIX shell) tricks ](http://www.etalabs.net/sh_tricks.html)
- [Shell productivity tips and tricks (2020)](https://blog.balthazar-rouberol.com/shell-productivity-tips-and-tricks.html) ([HN](https://news.ycombinator.com/item?id=22975437))
- [Tutorial - Write a Shell in C (2015)](https://brennan.io/2015/01/16/write-a-shell-in-c/) ([Code](https://github.com/brenns10/lsh))
- [DSL for shell scripting (2020)](https://acha.ninja/blog/dsl_for_shell_scripting/) ([Lobsters](https://lobste.rs/s/p6insb/dsl_for_shell_scripting))
- [Shell Script Compiler](https://github.com/neurobin/shc) - Generic shell script compiler. Shc takes a script, which is specified on the command line and produces C source code.
- [Shell script template suitable for most software developers](https://github.com/mjambon/reasonable-shell-script)
- [Chafa](https://github.com/hpjansson/chafa) - Command-line utility that converts all kinds of images, including animated GIFs, into sixel or ANSI/Unicode character output that can be displayed in a terminal.
- [streamhut](https://github.com/miguelmota/streamhut) - Stream and send data, terminal to web and vice versa.
- [TermBackTime](https://github.com/termbacktime/termbacktime) - Terminal recording and playback.
- [shell-functools](https://github.com/sharkdp/shell-functools) - Functional programming tools for the shell.
- [Hacking with environment variables](https://www.elttam.com/blog/env/) ([HN](https://news.ycombinator.com/item?id=23827486))
- [CMD.XYZ](https://cmd.xyz/) - GPT3 command creator for Linux.
- [Alacritty](https://github.com/alacritty/alacritty) - Cross-platform, GPU-accelerated terminal emulator. ([HN](https://news.ycombinator.com/item?id=24016977)) ([Lobsters](https://lobste.rs/s/ab8bfz/alacritty_version_0_5_0))
- [The Terminal Jockey's Toolbelt (2020)](https://packetlost.dev/the-terminal-jockeys-toolbelt) ([Lobsters](https://lobste.rs/s/8ax6zc/terminal_jockey_s_toolbelt))
- [asciicast2gif](https://github.com/asciinema/asciicast2gif) - Generate GIF animations from asciicasts (asciinema recordings).
