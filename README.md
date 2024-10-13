# totp

This is a CLI utility for managing TOTP keys and generating codes. It is written in PHP and has zero dependencies outside of the PHP standard library. All configurations are stored in ~/.totp

## Usage

Help info

```bash
Usage:
totp <name>   Generate code for named configuration
totp add      Interactively add a configuration
totp list     List configurations
totp all      Generate codes for all configurations
```

Add a configuration

```bash
$ totp add
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
