#### Usage: ####

Spin up a local copy of ubuntu using virtualbox and vagrant. Forwards
port 9999 to port 9000 on localhost. Provides remote execution against
the host.

`vagrant up`

`vagrant ssh`

`cd /vagrant`

`./persist.py -l -p 9999 -c`


From the host machine connect via telnet:

`telnet localhost 9000`

Any commands you run on the host vm are now executed against the VM.

#### Todo: ####

* Fix the client part of the script to execute properly in place
  of telnet.
* Add support and version checking for Python3.
* Add testing and build out into a PIP.

#### Notes: ####

This is a proof of concept based off of the book [Black Hat Python](https://nostarch.com/blackhatpython).