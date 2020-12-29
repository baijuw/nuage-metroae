# Metro Automation Engine Release Notes

## Release info

* MetroAE Version 4.3.0
* Nuage Release Alignment 20.10.R2
* Date of Release 29-Dec-2020

## Release Contents

### Feature Enhancements

* Support for deploying using Excel spreadsheet (.xlsx) files
* Add hosts and clusters folder support for vCenter (METROAE-1423)
* Add hook location for custom external certificates (METROAE-1424)
* Add support for IPv6 NUH install (METROAE-1416)
* Add support for Stats-out VSD deployements.
* Add example for CSV input spreadsheet (METROAE-1338)
* Support Inplace upgrades for Geo-redundant VSD
* Moved MetroAE container to Docker hub (METROAE-1430)
* Support for downloading container image from Docker hub (METROAE-245)
* Add NUH enhancements for VRRP, NTP and other NUH config (METROAE-1429)
* Add support for updating MetroAE Script during Container setup and update. (METROAE-1427)
* Add support for configuring only IPV6 environment in vcenter. (METROAE-276)
* Make MetroAE python scripts Python3 compatible (METROAE-1418)

### Resolved Issues

* Add support for IPv6 NUH install (METROAE-1416)
* Add NUH Deploy changes for license install prior to Config (METROAE-1422)
* Allow VSC to be specified without system ip (METROAE-1413)
* Added Serial=1 to prevent on VSD lockout of iptables during VSC's upgrade
* Fixed static route gateway issue in VNSUTIL
* Fixed issue with SDWAN Portal configuration (METROAE-244)
* Fixed the issue with VSD license with better error message when it expires (METROAE-1432)
* Add retries to yum update in case there are connection issues with repos
* Increased the retries for ejabberd connected users
* Skip testing for bootstrap complete when using activation link method

## Test Matrix

This release was tested according to the following test matrix. Other combinations and versions have been tested in previous releases of MetroAE and are likely to work. We encourage you to test this in your lab before you apply it in production.

Workflow | Target Server | Version
-------- | -------- | --------
Install | KVM | Geo-redundant 6.0.3
Install | KVM | HA 5.3.3
Install | KVM | HA 5.4.1
Install | KVM | HA 6.0.3
Install | KVM | Active-Standby ES 6.0.3
Install | KVM | HA IPv6 6.0.3
Install | KVM | SA 5.3.3
Install | KVM | SA 5.4.1
Install | KVM | SA 6.0.3
Install | KVM | Add VSC pair 6.0.3
Install | KVM | SA CPU pinning 6.0.3
Install | KVM | SA VNS end-to-end 6.0.3
Install | KVM | SA VNS multi-uplinks 6.0.3
Install | KVM | SA feature tests 6.0.3
Install | KVM | SA IPv6 6.0.3
Install | KVM | SA Terraform 6.0.3
Install | KVM | SA via Container 6.0.3
Install | OpenStack | HA 5.3.2
Install | OpenStack | HA 6.0.3
Install | OpenStack | SA 5.3.2
Install | OpenStack | SA 6.0.3
Install | vCenter | HA w/VCIN 6.0.3
Install | vCenter | HA w/Hybrid VCIN 6.0.3
Install | vCenter | HA 5.3.3
Install | vCenter | HA 5.4.1
Install | vCenter | HA 6.0.3
Install | vCenter | HA Custom passwords 6.0.3
Install | vCenter | SA 5.3.3
Install | vCenter | SA 5.4.1
Install | vCenter | SA 6.0.3
Install | vCenter | SA Custom passwords 6.0.3
Upgrade | KVM | Geo-redundant 5.4.1-6.0.3
Upgrade | KVM | HA 5.3.3-6.0.3
Upgrade | KVM | HA inplace 5.4.1-5.4.1U5
Upgrade | KVM | HA 5.4.1-6.0.3
Upgrade | KVM | HA hardened 5.4.1-6.0.3
Upgrade | KVM | HA inplace 6.0.3-6.0.5
Upgrade | OpenStack | HA 5.4.1-6.0.3
Upgrade | OpenStack | SA 5.4.1-6.0.3
Upgrade | vCenter | HA 5.4.1-6.0.3
Upgrade | vCenter | HA hardened 5.4.1-6.0.3
Upgrade | vCenter | HA inplace 5.4.1-5.4.1U5
Upgrade | vCenter | HA inplace 6.0.3-6.0.5
Upgrade | vCenter | SA hardened 5.3.3-6.0.3
Upgrade | vCenter | SA 5.4.1-6.0.3
Wizard Install | KVM | SA via container 6.0.3
Wizard Install | KVM | SA via CSV 6.0.3
Wizard Upgrade | KVM | SA 5.4.1-6.0.3
