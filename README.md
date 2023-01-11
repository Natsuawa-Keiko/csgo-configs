# CSGO-Configs

My *Counter-Strike: Global Offensive* settings.

Initial commit is directly copied from my another GitHub account due to privacy concern. If you accidentally find that account, please do not tell anyone else. Much appreciated.

## Q & A

### Where can I find my config directory?

By default, your config directory is located at `C:/Program Files (x86)/Steam/userdata/<your_steamID32>/730/local/cfg/`.

### Is it considered as game hacking?

No.

Config files save you in-game settings like keybindings, crosshair style, jumpthrow, etc. There is no difference between writing commands in your config files and executing them directly in the CSGO console. Commands like `sv_cheats 1` are server-side command and if your are not the host, your can run them whatever you want: they just **WILL NOT WORK**, and you will not considered as hacker but a dumb player.

### Can I just write them in the default `config.cfg`?

Yes, but not recommended.

CSGO client loads and saves your configuration by reading and writing `config.cfg`. After batch I/O operation, your `config.cfg` will be no longer read-friendly and hard to manage.

## Reference

[How to: Scripting, Binds and Configs](https://steamcommunity.com/sharedfiles/filedetails/?id=314801693)

[TOTAL CS:GO](https://totalcsgo.com/commands)
