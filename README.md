# Cloudbox-Commander
 A simple Bash script for cloudbox shortcuts.  <br /> <br />

Add this script named cloudbox to ~/.local/bin/ <br /> <br />

Proceed to use cloudbox as a command line interactive shortcut for installing applications with ansible or for doing other useful things on a cloudbox server. <br /> <br />

Interactive command line usaage is as such:  <br />
Simply run the command cloudbox. It will reply with the following options: <br />
 "m) Core Repo Installation - tag" <br />
 "c) Community Repo Installation -tag" <br />
 "s) Do a something" <br />
 "d) Dedupe a deduper -tag" <br />
 "u) Cloudplow upload" <br />
 "e) Exit" <br />


Direct Command line usage is as such: <br />
`cloudbox repo tagname (debug - optional/planned)` <br />
repo is a simple variable asking for M for main or C for community <br />
Examples: <br />
To install the plex tag you would use `cloudbox m plex`. This will run `cd ~/cloudbox && sudo ansible-playbook cloudbox.yml --tags plex`. <br />
To install the watchtower tag you could use `cloudbox c watchtower`. This will run `cd ~/community && sudo ansible-playbook community.yml --tags watchtower`. <br />
