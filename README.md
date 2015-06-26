# My Custom Vagrant Rails Development Setup
This is a custom rails development setup for Vagrant that I've pieced together to let me and a few friends have an easier time exploring Ruby.

# Requirements
### Installed
- Vagrant
- Virtualbox

# Usage
Drop the two files in this repository into a project folder, or parent folder:
- Vagrantfile
- Vagrant-setup/vagrant-postgres.sh

Run `vagrant up`

# Contents

### Image
`fitmentgroup/rvmruby222` is a custom image I've created based on `ubuntu/trusty64` with a few shortcuts:
- Ubuntu Server 14.04 x64
- Git from git-core ppa
- RVM
- Ruby 2.2.2
- Bundler

### Provisioned via `:shell`
- 1 GB ram
- PostgreSQL with Vagrant user
- Rails
- Ports forwarded:
  - 80 > 80       # typical http
  - 3000 > 3000   # rails webrick dev default
  - 5432 > 5432   # postgres

