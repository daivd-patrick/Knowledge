# [Hazel](https://www.noodlesoft.com)
I currently use Hazel to instantly commit any changes I make to CSV files of [web searches](https://github.com/nikitavoloboev/alfred-web-searches), [ask-create-share](https://github.com/nikitavoloboev/alfred-ask-create-share) as well as all of [LA's curated lists](https://github.com/learn-anything/curated-lists#readme). And essentially any kind of curated lists. I even automate commiting the README of [my macOS](https://github.com/nikitavoloboev/my-mac-os) repo as I want to instantly push any changes I make to the repo.

Since I want to keep my macOS repo always updated, I made a macro to open the README file in Sublime Text so I can quickly make a change, save and the change will instantly be commited with `update readme` message.

The rule for this is really simple and looks like this:
![](https://i.imgur.com/EF3elcv.png)

With this as the schell script:
![](https://i.imgur.com/eip64YV.png)

Here it is in code:
```bash
export USER=nikitavoloboev
if [ -e '/nix/var/nix/profiles/default/etc/profile.d/nix-daemon.sh' ]; then
   . '/nix/var/nix/profiles/default/etc/profile.d/nix-daemon.sh'
fi
git add README.md
git commit -m "update readme"
git push
```

The reason for the if statement there is that I use [Nix](../../package-managers/nix.md) package manager and my `git` command is installed with Nix so I want Hazel to use it. Otherwise it failed on my system.

## Notes
- If you want to have your rules to be applied onto subfolders as well as the directory chosen, add this rule.
![](https://i.imgur.com/yPfhkBo.png)

- If extensions are hidden, don't add extensions in the rule editor too.

## Links
- [Reference hazel file path](https://forum.keyboardmaestro.com/t/reference-hazels-file-path/9138)
- [Hazel Debug Mode](https://www.noodlesoft.com/kb/hazel-debug-mode/)