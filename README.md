1. Fork repository.

2. Create a  group_vars/all file.

```yaml
domain_name: example.com
ssl:
  src: files/certs
  cert_file: ssl.crt
  key_file: ssl.key
```

3. Create an inventory file.

```ini
[odoo]
example.com
```

4. Deploy with ansible.

```shell
$ ansible-playbook site.yml -i hosts
```
