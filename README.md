# Ansible Playbooks

Collection of Ansible playbooks for server configuration and application deployment.

## Playbooks

- `install_apache.yml` - Apache web server installation
- `install_nginx.yml` - Nginx web server installation  
- `docker.yml` - Docker installation and setup
- `multiENV_nginx.yml` - Multi-environment Nginx deployment

## Usage

```bash
# Using INI inventory
ansible-playbook -i inventory.ini <playbook-name>.yml

# Using YAML inventory
ansible-playbook -i inventory.yml <playbook-name>.yml

# Target specific environment
ansible-playbook -i inventory.yml <playbook-name>.yml --limit dev
```

## Inventory Files

- `inventory.ini` - Main inventory file
- `inventory.yml` - YAML format inventory
- `inverntory_env_nginx.ini` - Environment-specific Nginx inventory