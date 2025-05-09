This repo contains custom git commands for windows.

Write a custom shell command. Save it to file in C:\git-scripts. The

run this command in cmd

```git config --global alias.wip '!C:/git-scripts/wip'```

run this command in bash

``` git config --global alias.wip '!~/git-scripts/wip'```

Then use your custom command

```git retag V_10_2```
