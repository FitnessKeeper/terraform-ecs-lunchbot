Terraform Control repo built following

As outlines by Charity Majors in :
https://charity.wtf/2016/03/30/terraform-vpc-and-why-you-want-a-tfstate-file-per-env/

TLDR, but really, go read the post, it's way better then what I'm going to write here..


### use one of the current environments

- Clone the repo `git clone https://github.com/tfhartmann/terraform-ecs-lunchbot.git`
- `cd` into the base dir for the env you want to work on
  - `cd terraform-ecs-lunchbot/env-development/`
- `./init.sh` # to initialize your environment
- `terraform get` # to load your modules
- `terraform plan -var-file=development.tfvars` # manage all the things!
