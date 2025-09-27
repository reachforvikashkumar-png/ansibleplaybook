# ansibleplaybook
This repository provides a detailed guide to writing and executing Ansible playbooks using YAML. It includes explanations, examples, and practical use cases for automating system administration tasks.

# Intro
Ansible simplifies IT automation by allowing administrators to manage configurations and deployments using human-readable YAML syntax. This guide is designed to make it easier for users to write, understand, and execute Ansible playbooks effectively.

# About YAML n Syntax of Ansible Playbook
YAML stands for "Yet Another Markup Language."
Ansible uses YAML for defining playbooks because it is simple, human-readable, and concise compared to JSON or XML.
Example
---
name: My Ansible Playbook
hosts: all
tasks:
  - name: Create a directory
    file:
      path: /tmp/mydir
      state: directory
---

# File directory 
---
- hosts: demo
   tasks:
     - name: Create a directory
       file:
         path: /home/ansible/mydir
         state: directory
     - name: Create a file
       file:
         path: /home/ansible/myfile.txt
         state: touch
...
