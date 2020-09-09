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
```


## VPN

Create `/etc/vpnc.conf` following https://www.lrz.de/services/netz/mobil/vpnpda/. 

On host:
```
$ scp files/vpnc.conf polaris:~/vpnc.conf
$ scp ~/.ssh/config polaris:~/.ssh/config
```

On server:
```
$ sudo mv /home/jm/vpnc.conf /etc/vpnc.conf
$ sudo vpnc
```

