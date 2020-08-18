# Cloudbox-Commander
 A simple Bash script for cloudbox shortcuts.  <br /> <br />

Add this script named cloudbox to ~/.local/bin/ <br />
or (better) add a symlink from its location to  ~/.local/bin/cloudbox<br />
`ln -s ~/cloudbox-commandarr/cloudbox ~/.local/bin/cloudbox`

Proceed to use cloudbox as a command line interactive shortcut for installing applications with ansible or for doing other useful things on a cloudbox server. <br /> <br />

Interactive command line usaage is as such:  <br />
Simply run the command cloudbox. It will reply with the following options: <br />
 i) Show Server information as seen on login (MOTD) <br />
 m) Core Repo Installation - tag <br />
 c) Community Repo Installation -tag <br />
 a) List all ansible tags available to install<br />
 d) Dedupe with plex_dupefinder (must be installed) <br />
 u) Cloudplow upload <br />
 l) View Cloudbox logs<br />
 n) View Network info<br />
 d) View Docker container logs (not implemmeted yet)<br />
 e) Exit <br />


Direct Command line usage is as such: <br />
Many core interactive options are available as a direct command line argument. <br />
For example you can install a package from the cloudbox core or community packages: <br />
`cloudbox repo tagname (debug - optional/planned)` <br />
repo is a simple variable asking for M for main or C for community <br />
Actual Examples: <br />
To install the plex tag you would use `cloudbox m plex`. This will run `cd ~/cloudbox && sudo ansible-playbook cloudbox.yml --tags plex`. <br />
To install the watchtower tag you could use `cloudbox c watchtower`. This will run `cd ~/community && sudo ansible-playbook community.yml --tags watchtower`. <br />

It is possible to run a manual plex_dupefinder instance with: <br />
`cloudbox d`

or a manual cloudplow upload with:<br />
`cloudbox u`
