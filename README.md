Simple Ruby app deploy.

A .vault_password file should be created in the project root directory.

Download reqiurements:

`ansible-galaxy install -r requirements.yml`

Then start ansible playbook like this:

`ansible-playbook ansible-final-practice.yml --vault-id .vault_password`
