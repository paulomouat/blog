---
layout: post
title: "Setting up the dev environment"
date: 2012-08-14 18:35
comments: true
categories: ["Setup", "Git", "GitHub"]
---

To set up my dev environment on a brand new OS X 10.8 (Mountain Lion):

1.  If the SSH keys were not created, generate SSH key and add it to GitHub.
    1.  Instructions are available at <https://help.github.com/articles/generating-ssh-keys>.
    2.  On a brand new machine, there should be no pre-existing keys; if that is the case, jump directly to step 3,
        *Generate a new SSH key*.
    3.  Follow directions on step 4, *Add your SSH key to GitHub* and step 5, *Test everything out*. The system will ask
        for the key's passphrase, and you can add it to the keychain.

2.  Get the latest git from <http://git-scm.com/downloads/> and install it.

3.  In the projects folder, clone the devsetup repository to get the devsetup scripts:  
    
        $ git clone git@github.com:paulomouat/devsetup

4.  Clone the repos in GitHub by executing the following on the command-line:  
        
        $ ./devsetup/gitrepos.sh
