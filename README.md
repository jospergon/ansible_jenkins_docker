# run playbook in vagrant for testing purpose
vagrant up

# run playbook in amazon ec2
ansible-playbook site.yml -i inventory_file --private-key=~/.ssh/ci-server.pem -u ubuntu

add ciserver group to youe inventory file:

[ciserver]

your_server_dns_address_or_ip
