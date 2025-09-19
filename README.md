**Install the collection**
```bash
ansible-galaxy collection install netbox.netbox
```

```bash
virtualenv .venv
source .venv/bin/activate
pip3 install pytz pynetbox ansible
```

`ansible-playbook main.yaml`
