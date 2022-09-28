# SLURM ansible practice

A simple Ruby app with nginx and PostgreSQL.

A .vault_password file should be created in the project root directory.

Download requirements:

```
ansible-galaxy install -r requirements.yml
```
Create `.vault_password` file in the project root directory containing ssh password for the remote server.

Then start ansible playbook like this:

```
ansible-playbook ansible-final-practice.yml --vault-id .vault_password
```
