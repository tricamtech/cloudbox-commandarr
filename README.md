# cloudbox-commander
 Bash script for cloudbox shortcuts

Add this script named cloudbox to ~/.local/bin/

Proceed to use cloudbox as a command line interactive shortcut for installing applications with ansible or for doing other useful things on a cloudbox server.

for an interactive command line experience simply run the command cloudbox. it will reply with the following options.
 "m) Core Repo Installation - tag"
 "c) Community Repo Installation -tag"
 "s) Do a something"
 "d) Dedupe a deduper -tag"
 "u) Cloudplow upload"
 "e) Exit"


Direct Command line usage is as such:
`cloudbox repo tagname (debug - optional/planned)`
repo is a simple variable asking for M for main or C for community
Examples:
To install the plex tag you would use `cloudbox m plex`. This will run `cd ~/cloudbox && sudo ansible-playbook cloudbox.yml --tags plex`.
To install the watchtower tag you could use `cloudbox c watchtower`. This will run `cd ~/community && sudo ansible-playbook community.yml --tags watchtower`.
