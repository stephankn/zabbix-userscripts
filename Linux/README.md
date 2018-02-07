# Debian (based) systems

## Features
* checking whether a reboot is required (as requested by package updates)

## Compatibility
* Confirmed to work with Ubuntu 16.04 LTS (Xenial Xerus)

## Installation
* copy `debian.conf` to the agent include directory.
  Typically `/etc/zabbix/zabbix-agent.d/`
* Restart the agent:
      sudo systemctl restart zabbix-agent.service
* Import template `debian-template.xml` into Zabbix. Make sure to also import
  value mappings.
* Add template `Template OS Debian` to your hosts in addition to the
  probably already existing "Template OS Linux".

### Upgrade
* to upgrade replace the existing files with the newer versions.
  Re-apply any modifications done on top.
