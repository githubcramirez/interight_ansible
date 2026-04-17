# ansible-intersight-server-profile
Configure Server Profiles in Cisco Intersight

## Command Line Usage
Uses the Cisco Intersight Collection available at https://galaxy.ansible.com/cisco/intersight.  Here is example usage:
```
$ ansible-galaxy collection install cisco.intersight
$ cp example_imm_inventory inventory
<edit inventory with servers in your Intersight environment>
<add api_key_id and api_private_key variables to inventory OR set as environment variables:>
$ export INTERSIGHT_API_PRIVATE_KEY=/Downloads/SecretKey.txt
$ export INTERSIGHT_API_KEY_ID=596...
<for more information on key setup, see ansible-doc>
$ ansible-doc cisco.intersight.intersight_server_profile
<run the profile playbook>
$ ansible-playbook -i inventory intersight_server_profile.yml
```

## Ansible Tower Usage
If using Ansible Tower, this repo (or a clone) can be set as the Git SCM URL in your Project.  See https://youtu.be/TlNqHJbz5I4 for additional information on configuring and using Ansible Tower with Cisco Intersight.

