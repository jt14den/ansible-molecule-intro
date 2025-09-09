---
title: Setup
---

This lesson uses Ansible and Molecule to demonstrate automation and testing. Learners need a working Python environment, a way to run virtual machines or containers, and the required Ansible collections.

## Software Setup

::::::::::::::::::::::::::::::::::::::: discussion

### Details

We'll use Docker as the default driver for Molecule, though Vagrant can be substituted if you already use it.  
All operating systems will need Python, pip, and Git.  
We recommend creating a dedicated virtual environment for this lesson.  

:::::::::::::::: spoiler

### Windows

1. Install [Python 3](https://www.python.org/downloads/).  
2. Install [Docker Desktop](https://www.docker.com/products/docker-desktop/).  
3. Install [Git for Windows](https://git-scm.com/download/win).  
4. Open **PowerShell** or **Git Bash** for the exercises.  

::::::::::::::::::::::::

:::::::::::::::: spoiler

### MacOS

1. Install [Homebrew](https://brew.sh/).  
2. Install Python, Git, and Docker with:  
   ```bash
   brew install python git
   brew install --cask docker
   ```  
3. Open **Terminal.app** for the exercises.  

::::::::::::::::::::::::

:::::::::::::::: spoiler

### Linux

1. Use your package manager to install Python 3 and Git. For example on Ubuntu:  
   ```bash
   sudo apt update
   sudo apt install -y python3 python3-pip git
   ```  
2. Install [Docker Engine](https://docs.docker.com/engine/install/).  
3. Open your preferred terminal emulator for the exercises.  

::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::::::::::::::

## Ansible and Molecule

After Docker (or Vagrant) is set up, install the required Python packages:  

```bash
python3 -m venv ansible-env
source ansible-env/bin/activate
pip install ansible molecule molecule-docker
```

Install the Ansible collections used in this lesson:  

```bash
ansible-galaxy collection install community.docker ansible.posix
```
