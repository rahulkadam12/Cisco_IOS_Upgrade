
# Cisco IOS Upgrade

Upgrade the Cisco IOS to the latest version using Ansible.

## Note

- Before proceeding with automation make sure the current version of IOS is defined in group_vars/all.yaml file.
- You need to update the group_vars/all.yaml file with the IOS name - for e.g. - cat9k_lite_iosxe.16.12.04.SPA.bin
- Replace SCP, & Boot_Flash variable with the IOS name.
- Update the MD5 variable with the checksum value assiciated with the IOS(details can be found on Cisco website).
- Also, Update the IOS_Version varaible from the IOS name - e.g 16.12.04 as shown below.

## Steps 

- Check the current version of Cisco.
- Verify if the IOS version match with IOS_Version information provided in group_vars/all.yaml file.
- Add commands on the switch associcated to IOS Upgrade.
- Copy the IOS from the remote host to Flash using SCP 
- Verify the MD5 Checksum of the copied IOS.
- Boot the device with the new Verison of IOS.
- Wait for the device IP to come UP.
- Check if the current version is the same as the version defined in group_vars/all.yaml file.
- Send eMail to the Operations team.

## Contact

- Rahul Kadam
