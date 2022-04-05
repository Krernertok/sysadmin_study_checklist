# Sysadmin study checklist

## Server configuration
- System time
	- systemd-timesyncd + timedatectl
	- ntp
		- chrony?
- SSH
	- sshd configuration
- GRUB?
- BIOS?

## User management
- Users
- Groups
- Sudo

## File systems and storage
- Filesystem Hierarchy System
- Permissions
- LVM
- Relevant file system types
	- ext3, ext4
	- ?
- Network file systems
- Mounting, unmounting, fstab

## Backups
- Backup strategies
		https://www.msp360.com/resources/blog/guide-to-linux-patching-management/
		https://ubuntu.com/security/noticeshttps://ubuntu.com/security/notices
- Creating backups/snapshots
	- Minimizing downtime
	- backuppc
- Restoring from backups
	- Restore testing

## Installing, updating and patching software
- "Regular" software
	- apt-get, apt
		- adding sources
	- Installing package from file
	- Building from source
	- systemd unit files?
- OS updates
- Kernel updates
- Configuration management == Ansible

## System and process information
- top/htop
- ps
- vmstat
- sysstat?
- df + du

## Cron and systemd timers
- cron
	- cron syntax
	- crontab and different cron files
	- cron.allow and cron.deny
- systemd timers

## Networking and firewalls
- Networking principles
	- OSI model
	- Network topographies?
	- Internet
		- Protocols?
			- IP
			- TCP
			- UDP
		- DNS
- Proxies, NAT
- CIDR
- Interfaces
- iptables
- Relevant commands
	- netstat
	- telnet
- Physical networking like switches and links?

## Security
- Basics? Attack vector types?
- Hardening

## SSL Certificates
- Public key infrastructure
- Creating SSL certificates
	- Self-signed certificates
	- Let's Encrypt
- Testing certificates
	- openssl

## Logging
- Different logging systems
	- syslog
	- journald
- Rotation
- Log aggregation
	- ELK
	- Filebeat
	- Graylog

## Monitoring
- Zabbix
- Nagios?
- Prometheus?

## Webservers, proxies, load balancers
- nginx
- HAproxy
- httpd?

## Scripting and automation
- Mindset and principles
- CLI commands
	- awk?
	- sed?
	- grep
	- curl
- Shell scripting (bash, don't forget aliases!)
- Python
- Go

## Databases (=PostgreSQL)
- Installation, configuration
- Creating tables, users
- Tuning?
- NoSQL databases
	- redis
	- mongodb

## Virtualization and containers
- vagrant
- KVM?
- Docker
- Kubernetes

## VCS
- git
- Gitlab, Bitbucket, ?

## CI/CD
- Jenkins
- Gitlab
- ?

## Artifact store
- Artifactory
- Sonatype Nexus?

## Cloud
- Terraform
- AWS
- Azure
- GCP?

## Extras
To be curated:
- vim
	- Substitution
	- Registers
	- Buffers
	- Macros
	- Tabs, windows, split editing
	- Marks, global marks
	- Configuration
	- Running commands
- tcpdump
- strace
- rsync
- tee
- tmux
- xargs
- ncat
- iftop
- iptstate
- screen
- pdsh
- logtail
- dstat
- mysqltuner
- bacula
- mrxvt
- ccze
- rzip
- cpipe
- column
- tput
- iotop
- renice
- ionice
- parallel
- multitail
- grc
- borgbackup
- zstd
- pv
- keychain
- findmnt
- lxc
- htop
- tigervnc
- xpra
- lsyncd
- ncdu
- oping
- gdu
- synergy
- alacritty
- terminator 
