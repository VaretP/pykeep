# Pykeep

Keep your config files at the same place and edit them without changing directory.

# Usage

## First time setup

```
$ git clone https://github.com/Dirtyhenki/pykeep
$ chmod +x pykeep
$ ./pykeep -f 
```

Then edit the file `conf.pykeep`

```
$ ./pykeep -i
```
And you're all set. Use `./pykeep` to update your files. 

Pykeep keeps a copy of the files you edited in their directory, for example if you edit `i3config` and you have in your conf.pykeep this line : `"i3config" > "../.config/i3/config"` then when you launch pykeep it will create a file called `config_old` in `../.config/i3/config`.
