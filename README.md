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


## Development

Needs `python3-winrm`, or `python2-winrm`
