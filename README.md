# PixelWise — Ansible Playbook Migration

This repository contains my project work for the course Methoden und Werkzeuge der Softwareentwicklung. The goal was to take the existing `setup-server.sh` Bash script that provisions the PixelWise server and rebuild it as an Ansible playbook.

## What is in this repo

- `setup-server.sh` — the original Bash script that serves as the baseline
- `ansible/` — the Ansible playbook
  - `playbook.yml` — covers the same eight deployment responsibilities as the Bash script
  - `inventory.yml` — defines the host group `pixelwise`
  - `ansible.cfg` — Ansible configuration, including SSH pipelining
- `measurements/` — the run logs and static analysis outputs referenced in the report
  - three runs each for the Ansible playbook and the Bash script
  - one log per linter (`ansible-lint`, `yamllint`, `shellcheck`)

## How to run the playbook

From the `ansible/` directory:
