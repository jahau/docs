# Install 
the first step in using the nebulactl CLI tool is to install it, you do that by running the following command on a 64bit Linux OS: 

```bash
sudo wget https://github.com/nebula-orchestrator/nebula-cmd/raw/master/dist/nebulactl -O  /usr/local/bin/nebulactl && sudo chmod +x /usr/local/bin/nebulactl
```

this install a single bin file in the /usr/local/bin path which makes it accessible from any path in the shell.

# Login
after installing "nebulactl" you have to configure it by pointing it to your cluster, you do it by running the following command

```bash
nebulactl login --username <root> --password <password> --host <nebula.host.com> --port <80> --protocol <http/https>
```

or if you prefer a guided questions login just run:

```bash
nebulactl login 
```

either of this 2 methods creates a file in ~/.nebula.json with the login details, nebulactl checks this file every time it runs a command against the nebula API, also note that the file is per user so if you have multiple users you will have to either copy this file or run the `nebulactl login` command for each of them

# Use
the --help argument will give you the needed parameters for each command, most commands will also prompt interactively if a required parameter is missing to ease first time users.

```bash
nebulactl --help

Usage: nebulactl.py [OPTIONS] COMMAND [ARGS]...

  Connect to a Nebula orcherstrator management endpoint, Create Nebula apps
  and Manage them all from a simple CLI.

Options:
  --version  Show the version and exit.
  --help     Show this message and exit.

Commands:
  apps           Manage nebula apps.
  device-groups  Manage nebula device_groups.
  login          login to nebula
  logout         logout of nebula, useful when you want to make sure to...
  ping           check nebula api responds
  prune          Prune images.
  reports        List nebula device reports.
  user-groups    Manage nebula user groups.
  users          Manage nebula users.

```
