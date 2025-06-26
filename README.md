## 👋 Welcome to whois 🚀  

Description

### Requires scripts to be installed

```shell
sudo bash -c "$(curl -q -LSsf "https://github.com/dfmgr/installer/raw/main/install.sh")" && sudo dfmgr install installer
```

### Install docker compose files

```shell
composemgr install whois
```

### Edit .env

```shell
$EDITOR "$HOME/.config/myscripts/composemgr/docker/$whois/.env"
```

### Edit app.env - will overwrite defaults from .env

```shell
$EDITOR "$HOME/.config/myscripts/composemgr/docker/$whois/app.env"
```

### Pull the containers

```shell
composemgr --dir "$HOME/.config/myscripts/composemgr/docker/$whois" pull
```

### Start the stack

```shell
composemgr --dir "$HOME/.config/myscripts/composemgr/docker/$whois" up &&
```

### Get the logs for the stack

```shell
composemgr --dir "$HOME/.config/myscripts/composemgr/docker/$whois" logs
```
