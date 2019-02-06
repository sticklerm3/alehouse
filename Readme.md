# alehouse

My custom zsh-plugin for `zsh` inspired by [betterbrew][8a51380c].

`alehouse-zsh-plugin` contains short aliases for homebrew commands. For now I just have the ones from my personal `.aliases` file and those from [betterbrew][8a51380c].

This is for my personal use and is always a work in progress. Feel free to use it, and dont be afraid make suggestions or offer any corrections to mistakes!

## Example

Without typing full homebrew commands in console, like:

```sh
$ brew install zsh --build-from-source
```

there is more convenient alias:

```sh
$ bifs zsh
```

## Installation on oh-my-zsh

1. Go to `oh-my-zsh` plugins directory:

```sh
$ cd ~/.oh-my-zsh/custom/plugins
```

2. Clone the repository into a new directory `alehouse` :

```sh
git clone https://github.com/sticklerm3/alehouse-zsh-plugin.git alehouse
```

3. Enable `alehouse` plugin by adding to your `.zshrc` configuration file:

```sh
$ plugins=(alehouse)
```

4. Restart your shell.

```sh
$ source .zshrc
```

## Brew every day

The best part of waking up is having shortcuts in your cup!

| alias    | command                                                                                 |
| :------- | :-------------------------------------------------------------------------------------- |
| `cask`   | `brew cask`                                                                             |
| `brewup` | `brew -v update && brew -v upgrade && brew cask upgrade && brew cleanup && brew doctor` |

## All Aliases

### My additions

| personal | Command             |
| :------- | :------------------ |
| `bi`     | brew info\*         |
| `bis`    | brew install        |
| `bs`     | brew search         |
| `bsd`    | brew search --desc  |
| `cask`   | brew cask           |
| `ci`     | cask install        |
| `cus`    | brew cask uninstall |
| `cuz`    | brew cask zap       |
| `blv`    | brew leaves         |

> - `bi` currently conflicts with the bundler package currently included with omz. Comment this out if you prefer to use that one.

### betterbrew aliases

> aliases that are ~~crossed out~~ have been removed.

| betterbrew   | Command           |
| :----------- | :---------------- |
| `binst`      | brew install      |
| `buinst`     | brew uninstall    |
| `bupd`       | brew update       |
| `blst`       | brew list         |
| `bsrch`      | brew search       |
| `banal`      | brew analytics    |
| `bcat`       | brew cat          |
| `bclean`     | brew cleanup      |
| `bcom`       | brew command      |
| `bcoms`      | brew commands     |
| `bcon`       | brew config       |
| `bdeps`      | brew deps         |
| `bdesc`      | brew desc         |
| `bdiy`       | brew diy          |
| `bdoc`       | brew doctor       |
| `bfetch`     | brew fetch        |
| `bgist`      | brew gist-logs    |
| `bhome`      | brew home         |
| `binfo`      | brew info         |
| `bleaves`    | brew leaves       |
| `bln`        | brew ln           |
| `blog`       | brew log          |
| `bmig`       | brew migrate      |
| `bmiss`      | brew missing      |
| `bopt`       | brew options      |
| `bout`       | brew outdated     |
| `bpin`       | brew pin          |
| `bpinst`     | brew postinstall  |
| ~~`bprune`~~ | ~~brew prune~~    |
| `bread`      | brew readall      |
| `brinst`     | brew reinstall    |
| `bsh`        | brew sh           |
| `bstyle`     | brew style        |
| `bswitch`    | brew switch       |
| `btap`       | brew tap          |
| `btapinfo`   | brew tap-info     |
| `btappin`    | brew tap-pin      |
| `btapunpin`  | brew tap-unpin    |
| `bulink`     | brew unlink       |
| `bupack`     | brew unpack       |
| `bupin`      | brew unpin        |
| `butap`      | brew untap        |
| bupdr        | brew update-reset |
| `bupgr`      | brew upgrade      |
| `buses`      | brew uses         |
| `bcache`     | brew --cache      |
| `bcell`      | brew --cellar     |
| `benv`       | brew --env        |
| `bprefix`    | brew --prefix     |
| `brepo`      | brew --repository |
| `bver`       | brew --version    |

To-do:

- [ ] replace alias for `brew prune` as its been deprecated.
- [ ] re-organize cheatsheet to be sorted by category.

[8a51380c]: https://github.com/timothyrowan/betterbrew-zsh-plugin "betterbrew on github"
