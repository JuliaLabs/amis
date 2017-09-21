# Introduction
This repository holds the necessary script to build and deploy the AMIs provided by JuliaLabs@MIT

## Instructions
1. Configure the AWS cli
   - You might also want to note your AWS User ID
   - and VPC subnet
   - customise the `*.json` files to use these
2. Install packer.io and ansible
3. `packer build juliabase.json` to create a base Julia AMI
4. Customise `REQUIRE` and `juliagpu_playbook.yml` to include everything you need.
5. `packer build juliagpu.json`
6. Go online and make your new AMI public.
