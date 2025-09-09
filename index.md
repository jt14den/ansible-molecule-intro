---
site: sandpaper::sandpaper_site
---

# Getting Started with Ansible and Molecule

This lesson introduces **Ansible** for infrastructure automation and **Molecule** for testing and validating Ansible roles.  

It is designed for people who have some experience with virtual machines or containers but are new to infrastructure-as-code. By working through the lesson, you will learn how to automate system configuration and test your work before deploying to production.

## Objectives

- Explain the benefits of infrastructure-as-code for reproducibility and collaboration  
- Run an Ansible playbook to install and configure software on a VM or container  
- Describe the role of **idempotence** in configuration management  
- Write and organize Ansible roles with variables and defaults  
- Use **Molecule** to create, converge, and test an Ansible role  
- Diagnose and resolve common Ansible and Molecule errors  
- Apply knowledge to build a minimal reproducible infrastructure component (e.g., Apache or Postgres)  

## Prerequisites

::: prereq
- Comfort using the command line (basic navigation, editing files, running commands)  
- Some prior experience with virtual machines or containers (e.g., Docker, Vagrant, or cloud VMs)  
- Ansible, Python, and Docker installed (setup instructions provided in this lesson)  
:::
