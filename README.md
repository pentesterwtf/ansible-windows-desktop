# Desktop Deploy

* Ansible script to deploy a Windows 10 / Server 2019 host
* Also usable for development VM's
  * Like <https://github.com/pentesterwtf/packer-windows>

## Breakdown

See individual roles under `roles/`

## Development

* Needs `python3-winrm`, or `python2-winrm`
* Needs molecule / molecule vagrant / molecule libvirt
* Will pull down a server2019/Win10 image and test end-to-end against both
* See `molecule/default`
  * Takes forever to spin up - PR's welcome if you can figure out why :)


# REMOVE THE BELOW



# Desktop Deploy (Windows)

* Dodgy ansible script to setup my Windows 10 desktop
* Also used for development VMs
  * Like <https://github.com/pentesterwtf/packer-windows>

## Breakdown

### Common role

* Putty
* Google Chrome
* vscode
* sysinternals

### Defender disable cloud

* Disables the automatic cloud submission for defender
* Perhaps handy if you're testing :)

### Logging role

* Sysmon

### Reveng role

* Ghidra
* 010editor
* die
* explorersuite
* dnspy
* ilspy


### Fireye

* Adds the chocolately repository used by fireeye's commando-vm
* See https://github.com/fireeye/commando-vm


