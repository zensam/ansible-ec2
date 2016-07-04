# ansible-ec2
Ansible and AWS EC2 stuff

#### Commands to run playbooks

```bash
sudo pip install boto
```

##### Set AWS credentials in *``boto``* user config:  
```bash
vi ~/.boto
```
```
[Credentials]
aws_access_key_id = <enter your aws access key id here>
aws_secret_access_key = <enter your aws secret key here>
```
##### Clone git repo:

```bash
git clone https://github.com/zensam/ansible-ec2.git
cd ansible-ec2/vpc
ansible-playbook -vvv -i localhost, -e "type=all" pb-vpc.yml
```


#### Dynamic inventory

```bash
cd /etc/ansible
sudo wget https://github.com/ansible/ansible/blob/stable-2.1/contrib/inventory/ec2.py
sudo wget https://github.com/ansible/ansible/blob/stable-2.1/contrib/inventory/ec2.ini
sudo chmod +x ec2.py
```

```bash
cd /etc/ansible
sudo wget https://raw.githubusercontent.com/yankurniawan/ansible-for-aws/master/ec2.py
sudo wget https://raw.githubusercontent.com/yankurniawan/ansible-for-aws/master/ec2.ini
sudo chmod +x ec2.py
```
