# CS:GO Configs

My *Counter-Strike: Global Offensive* settings.

Initial commit is directly copied from my another GitHub account due to privacy concern. If you accidentally find that account, please do not tell anyone else. Much appreciated.

## Before We Start

### What are the path components?

Assume we have a file named `/foo/bar/example.txt`, then

- parent: `/foo/bar/`
- filename: `example.txt`
- stem: `example`
- suffix: `.txt`
- extension: `txt`

Note that the path aforementioned is in Posix-style. Windows uses backslash `\` as its path separator but slash `/` is also compatible. From now on we only talk about paths in Posix-style.

### Make your file suffixes visible!

If not, when you create a file named `autoexec.cfg`, it may actually be like `autoexec.cfg.txt`, with its suffix `.txt` hidden.

Click [here](https://support.microsoft.com/en-us/windows/common-file-name-extensions-in-windows-da4a4430-8e76-89c5-59f7-1cdbbc75cb01) for more information.

### How will a file be affected by its suffix?

A common misunderstanding is that we can change the type of a file by changing suffix, which is not true. Actually, suffixes are only for the operating system to infer which software/program should be called to open files, and has nothing to do with the data of the file.

CS:GO client chooses `.cfg` as its config files' suffix, and a `.cfg` file is literally **OF NO DIFFERENCE** from a `.txt` file. So don't be scared!

### Where can I find my config directory?

By default, your config directory is located at

```
C:/Program Files (x86)/Steam/userdata/<your_steamID32>/730/local/cfg/
```

### Is it considered as game hacking?

No.

Config files save you in-game settings like keybindings, crosshair style, jumpthrow, etc. There is no difference between writing commands in your config files and executing them directly in the CS:GO console. Commands like `sv_cheats 1` are server-side commands and if your are not the host, your can input and execute them whatever you want: they will just **NOT WORK**, and you will not considered as a hacker but a dumb player.

### Can I just write them in the default `config.cfg`?

Yes, but not recommended.

CS:GO client loads and saves your configuration by reading and writing `config.cfg`. After batch I/O operation, your `config.cfg` will be no longer read-friendly and hard to manage.

A better implementation is that writing down you settings in a file named `autoexec.cfg`. This file is expected to execute automatically, if not, add `+autoexec` to your CS:GO launch option.

## Reference

- [How to: Scripting, Binds and Configs](https://steamcommunity.com/sharedfiles/filedetails/?id=314801693)

- [TOTAL CS:GO](https://totalcsgo.com/commands)
