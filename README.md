# Desktop Deploy

* Ansible script to deploy a Windows 10 / Server 2019 guest
* This is mostly for RE/.NET nonsense
* Also usable for development VM's

## Usage

Don't like Vagrant? See <https://github.com/pentesterwtf/windows-terraform>

## Breakdown

See individual roles under `roles/`

## Development

* Needs `python3-winrm`, or `python2-winrm`
* Needs molecule / molecule vagrant / molecule libvirt
* Will pull down a server2019/Win10 image and test end-to-end against both
* See `molecule/default`
  * Takes forever to spin up - PR's welcome if you can figure out why :)
