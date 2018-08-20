## Private repo for sensitive issue repros

Use this repo to create Terraform configurations that might be sensitive
(contain customer information / resource names) and that need to be repro'd in
Terraform Enterprise rather than locally. Make a branch for your repro and
integrate this repo and your branch with Terraform Enterprise.

1. Create a branch with the ticket number (e.g. `git checkout -b 6111`)
2. Add your configuration (e.g. `vim main.tf`, `git add main.tf`)
3. Push your branch to Github (e.g. `git push -u origin 6111`)
3. Create a workspace in TFE
4. Add this repo and specify that the integration should use your branch
5. Carry on with the repro
