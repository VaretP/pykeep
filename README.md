# Pykeep

Keep your config files at the same place and edit them without changing directory.

# Usage

## First time setup

```
$ git clone https://github.com/Dirtyhenki/pykeep
$ cd pykeep/
$ ./pykeep -f 
```

Then edit the file `conf.pykeep` and run :

```
$ ./pykeep -i
```
And you're all set. Use `./pykeep` to update your files. 

Pykeep keeps a copy of the files you edited in their directory, for example if you have in your conf.pykeep this line : `"i3config" > "../.config/i3/config"` and you edit `i3config` then when you launch pykeep it will create a copy of `config` called `config_old` in `../.config/i3/config`. 

## Options

`$ ./pykeep -i f1 f2` overwrites files `f1, f2, (etc..)` with your actual config files. With the past exemple if you type `$ ./pykeep -i i3config` it will replace `i3config` by `../.config/i3/config`

`$ ./pykeep -b f1 f2` (etc..) replace your actual config files with their last version (.Yourfile_old). You can recall it to cancel.

`$ ./pykeep -h` Only gives the link of the repo.

## Screenshot

![config](https://i.imgur.com/dBU57sx.png)
