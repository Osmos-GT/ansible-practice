# SLURM ansible practice

A simple Ruby app with nginx and PostgreSQL.

Create `.vault_password` file in the project root directory containing your credentials:
```
my_centos_sudo_pass: <pass>
my_centos7_sudo_pass: <pass>
gitlabuser: <pass>
gitlabpassword: <pass>
```

Then start ansible playbook like this:

```
ansible-playbook ansible-final-practice.yml --vault-id .vault_password
```
