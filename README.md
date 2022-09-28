# SLURM ansible practice

A .vault_password file should be created in the project root directory.

Download requirements:

`ansible-galaxy install -r requirements.yml`

Then start ansible playbook like this:

`ansible-playbook ansible-final-practice.yml --vault-id .vault_password`
