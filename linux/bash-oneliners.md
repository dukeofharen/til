### Extract .tar.gz
```
tar xvzf file.tar.gz -C /path/to/dir
```

### Get .sh script directory
```
DIR="$( cd "$( dirname "${BASH_SOURCE[0]}" )" >/dev/null 2>&1 && pwd )"
```

### .bashrc

Adding lines to $HOME/.bashrc makes sure these lines are executed whenever a new terminal session is started.

### Start ssh agent for GIT
```
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/git.id_rsa
```

### Use different SSH private keys 
Source: https://stackoverflow.com/questions/2419566/best-way-to-use-multiple-ssh-private-keys-on-one-client
`.ssh/config`

```
IdentityFile ~/.ssh/id_rsa
IdentityFile ~/.ssh/id_rsa_old
IdentityFile ~/.ssh/id_ed25519
```

### SSH use different port

```
ssh user@192.168.1.1 -p 26
```

### Create SSH tunnel

```
ssh -L 3307:host.nl:3306 -p 1122 user@host.nl
```

### SCP copy file to host

```
scp -P 2908 user@host.nl:/tmp/sql_backup.sql ~
```

### SCP copy file to server

```
scp -P 2908 user@host.nl:~ /tmp/sql_backup.sql
``` 