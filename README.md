## Colorless preview of user and super user bash prompts.
### Custom coloring includes:
  ### username and hostname - olive drab green
  ### jobs, exit prompts, and current working directory - amber
  ### job number and exit code - red
  ### blue accent colors

User Display
```bash
┌─╼[Islc12@my-workstation]-[~/Documents]
└───╼[jobs:(0) exit:(0)]-$
```

Root Display
```bash
┌─╼[root@my-workstation]-[/var/log]
└───╼[jobs:(0) exit:(0)]-#
```

### Jobs display shows the number of backgrounded jobs.

### Exit diplay shows the exit code from the last used command, the same result can be found by doing `$?`.

## Installation
```bash
git clone https://github.com/Islc12/bash-ps1.git
cat bash-ps1/custom_ps1 | sudo tee -a ~/.bashrc /root/.bashrc
source ~/.bashrc
```
