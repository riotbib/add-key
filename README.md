add-key
=======

`add-key` allows adding SSH keys to the SSH agent, while not having to
remember every passphrase. You may source them from your password
manager. It passes the passphrases to `ssh-add` via `sshpass`.

## Install

```bash
$ # Add to PATH
$ cp add-key $HOME/bin/
$ # Adjusting config
$ mkdir $HOME/.config/add-key
$ cp config.ini.example $HOME/.config/add-key/config.ini
$ vim $HOME/.config/add-key/config.ini
```

## Usage

```bash
$ add-key
Usage: ./add-key main
```

## Dependencies

- `sshpass`, [Source](https://sourceforge.net/projects/sshpass/)

## Known bugs

- Passphrases may not contain quotation marks and some other special
  characters.
