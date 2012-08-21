---
layout: post
title: "Setting up the command for Sublime Text 2"
date: 2012-08-20 21:05
comments: true
categories: [Setup, Sublime Text]
---

To set up the command-line script to invoke Sublime Text 2 do the following:

1.  In the **devsetup** repo, grant the **create_subl_symlink.sh** script execution rights:

        $ chmod a+x create_subl_symlink.sh

2.  Execute the script:

        $ ./create_subl_symlink.sh

3.  Sublime Text 2 can now be invoked from the command-line by simply executing 

        $ subl

    or

        $ subl <name of file to edit or create>