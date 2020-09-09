# ansible_workstation

## Prerequisits

Clone this repository, install ansible and dependencies:
```commandline
$ ansible-galaxy install -r requirements.yml -f
```


## Usage

```
$ ansible-playbook -u root basic_setup.yml
$ ansible-playbook provision.yml
$ dropbox start -i
$ dropbox start
$ dropbox autostart y
```


## VPN

Create `/etc/vpnc.conf` following https://www.lrz.de/services/netz/mobil/vpnpda/.

