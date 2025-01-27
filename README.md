Creating a custom git command in Windows
create a cmd/bat file with the command. E.g. retag.cmd, save it in C:\git-scripts for example

add your git commands to the file. For example, this set of commands deletes the specified tag from your current branch both locally and remotely, then tags it with the same tag and pushes the change remotely

git tag -d %1

git push origin :refs/tags/%1

git tag %1

git push origin tag %1

run this command from your console

git config --global alias.retag '!C:/git-scripts/retag.bat'

use your custom command

git retag V_10_2