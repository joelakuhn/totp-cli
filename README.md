# totp

This is a CLI utility for managing TOTP keys and generating codes. It is written in PHP and has zero dependencies outside of the PHP standard library. All configurations are stored in ~/.config/totp-cli.

## Usage

Help info

```bash
$ totp -h
Usage: totp [name...]
totp -i, --insert   Interactively add a configuration
totp -l, --list     List configurations
totp -a, --all      Generate codes for all configurations
totp -r, --remove   Remove configuration
totp -h, --help     Show usage
```

Add a configuration

```bash
$ totp -i
name: example 
secret: N5UCYIDZN52SO4TFEBZW6IDDN5XWYIIK
passphrase length [6]: 
period [30]: 
```

Generate current code

```bash
$ totp example
749023
```

List configs

```bash
$ totp -l
example
```

Generate codes for all configs

```bash
$ totp -l
example:        745172
```

Generate codes for all configs

```bash
$ totp -r exmple
Remove `/Users/joel/.config/totp-cli/example.ini`? [Y/n]: 
```
