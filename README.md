# Ansible Playbooks

This repository contains a collection of Ansible playbooks designed to automate routine tasks.
Currently, it includes a single playbook for installing Docker, with plans to add more in the future.

## Playbooks

### `install_docker.yml`

Installs and configures Docker on the target host.
This playbook is primarily used as part of a Jenkins job, but it can also be run manually.

## Usage

### Prerequisites

* Ansible installed on your control machine
* Access to the target host(s) via SSH
* Sudo privileges on the target host(s)

### Running the playbook

```bash
ansible-playbook -i inventory install_docker.yml
```

Replace `inventory` with your inventory file containing the target hosts.

## Roadmap

* Add playbooks for other common setup tasks
* Improve integration with Jenkins pipelines

---

