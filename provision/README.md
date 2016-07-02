## Provisioning EC2 instances with ansible

**Usage:**

###### Create a variables file using *ec2_vars/testnodes.yml* as a template.

```bash
vi ec2_vars/testnodes.yml
```

###### After setting all variables, run it:

```bash
ansible-playbook -vv -i localhost, -e "type=testnodes" provision-ec2.yml
```
