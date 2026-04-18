run playbook by

`` ansible-playbook -i inventory.ini [playbook].yml ``

# ‼️ Important before running

Be sure to check 
[ ] playbook.yml
[ ] playbook-vm-config.yml
[ ] inventory.ini
[ ] ssh private key in the folder

remove all # comment and replace the placeholder value preceeding them with your own value

# Intended flow

1. Create Proxmox VM template ([guide](https://docs.google.com/document/d/1rugRbAGY0BACRm1YzdM2rtt1QqFCidJpAVAVOzcMRmo/edit?tab=t.0))
2. Replace playbook.yml variables with your own variable (lines with #)
3. Run `` ansible-playbook -i inventory.ini playbook.yml ``
4. Wait for ansible to finish
5. Check the VM is created on proxmox
6. Get the IP address from the newly created VM and replace the inventory.ini and playbook-vm-config.yml
7. Replace playbook-vm-config.yml variables
8. Run `` ansible-playbook -i inventory.ini playbook-vm-config.yml ``
9. ssh to the new VM and check if hostname is changed

feel free to reach out to Electric Nutbuster on discord for issue

rule is not used right now. because we don't need to reuse docker install rule.


All my SRE related archives:

# Site Reliability Engineering (SRE) & System Ops

## Full Capstone Overview
* [Capstone report on Site deployment](https://docs.google.com/document/d/15Hzd9wjUsI2Zh6n5f0O6Cs9WdtLblnv9dQ_frlJLkfI/edit?tab=t.0)

## Guides and HowTo for everyone
* [How to create template for Ubuntu Cloud-init on Proxmox](https://docs.google.com/document/d/1VTU_fT-Q2j417OONdcVRyHn8XKupkVmZOhkHYJMysKs/edit?tab=t.0)
* https://docs.google.com/document/d/1M2Qh4g64lcx9nue_O2gK1-UlUgS_wD56dwGl_fxGFnw/edit?tab=t.0
https://docs.google.com/document/d/1rugRbAGY0BACRm1YzdM2rtt1QqFCidJpAVAVOzcMRmo/edit?tab=t.0
https://docs.google.com/document/d/17spXrl8xwBoOvrH6X-tVfNCbyj9BZocAPJcfO4DS5FE/edit?tab=t.0
## Runbooks
* [Risk Assessment & Service Reliability](https://docs.google.com/document/d/1C1raS7NSXc3XHKfNUEvt97Pvv3hU4yFnicLSKIZ0lMI/edit?tab=t.0)
* [Risk Assessment & Service Reliability](https://docs.google.com/document/d/1nKWm3i1VpGTHOY6veufgIwL5YRX1HE4sv6HfNQQmf8Y/edit?tab=t.0)
https://docs.google.com/document/d/1_LAWtMcgnUvijLHUrJFM4DqlRlR32-lLSV1GdMjIi_4/edit?tab=t.0
## Postmortems
* https://docs.google.com/document/d/1-0X2nka6iVPxfIG6Som3wJdGZ-n_KnFQbz9Z68xdgzA/edit?tab=t.0
https://docs.google.com/document/d/12GOoi3Gh1_qZtJavcAg6A9IlPtCFLvwxJRzDh1KBrfE/edit?tab=t.0
https://docs.google.com/document/d/1HlRrIKjjywx6X6psb91P5HaxJ4jPBzSIu6gkg9IsoRk/edit?tab=t.0
## Investigations and Troubleshooting
https://docs.google.com/document/d/1VDrZj2v8v1r7LUu5BeqFG7Kck1EDrCz4DCu6ygxqrqA/edit?tab=t.0
