Set of tools to make COD7 more useful for conference planning.

In particular, the additions are aimed at making versions alpha2 and higher easier to use. COD 7alpha2 is the line that integrates OG, which brings with it both more powerful functionality, at the cost of some development pain. This module aims to bridge that gap.

Originally developed for NYC Camp website (http://nyccamp.org) with the intent of releasing back to COD community.

NB: Since NYC Camp is a 100% free event, initial Codify tools do not address paid registration issues.

##This repository contains a Vagrantfile.
####If you would like to load NYC-Camp 2014 in a Vagrant box, do the following (in brief):


  1. `git clone` this repo into a directory on your local machine.
  2. Install Vagrant
  3. Ensure you are running a 64-bit CPU with VT-x hardware virtualization enabled in the BIOS.
  4. Get a copy of the latest NYC-Camp 2014 Drupal database and rename it "nyccamp2014.sql" in the root of your git clone
  5. In a terminal, `cd` into your cloned repository
  6. Run `vagrant up --provision`. This should take a while.
  7. When the `vagrant up` command finally dumps you back into a command prompt, assuming there were no errors, type `vagrant ssh` and you will be ssh'd in to the box.
  8. NYC-Camp 2014 should be visible by visiting http://localhost:8080 in your browser. It also will listen on "nyccamp2014.local:8080" and "nyccamp2014:8080" if you wanna set those up in your hosts file.
  9. If you are SSH'd into your vagrant box, you should be able to see the webroot at /var/www
  10. If you are in the webroot, you may need to run `drush updb` before the site will function properly.
  11. The database should be loaded into "nyccamp2014" with user "nyccamp2014" and password "nyccamp2014".

@TODO- Featurize session grid views.
