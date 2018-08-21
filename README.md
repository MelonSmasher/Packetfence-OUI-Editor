# OUI Editor for Packetfence

## Install

```bash
# grab the code
cd /opt; 
git clone https://github.com/TheSageColleges/Packetfence-OUI-Editor.git;
cd Packetfence-OUI-Editor;
# Move the oui text file locally to avoid losing changes between upgrades
mv /usr/local/pf/conf/allowed_device_oui.txt /opt/Packetfence-OUI-Editor/oui.txt && ln -s /opt/Packetfence-OUI-Editor/oui.txt /usr/local/pf/conf/allowed_device_oui.txt;
# make the script available globally
ln -s /opt/Packetfence-OUI-Editor/ouiadd /usr/local/bin/ouiadd;
```

## Usage

```bash
ouiadd 00:11:22 Xbox
```

This would add an oui for xboxes

