- Fork repository.
- Create a  group_vars/all file.
```yaml
domain_name: example.com
ssl:
  src: files/certs
  cert_file: ssl.crt
  key_file: ssl.key
```
- Create an inventory file.
```ini
[odoo]
example.com
```
- Deploy with ansible.
```shell
$ ansible-playbook site.yml -i hosts
```
