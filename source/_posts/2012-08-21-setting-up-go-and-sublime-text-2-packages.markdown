---
layout: post
title: "Setting up Go and Sublime Text 2 packages for editing Go code"
date: 2012-08-21 21:36
comments: true
categories: [Setup, Go, Sublime Text]
---

Instructions to download and install the Go tools are available at <http://golang.org/doc/install>, but in essence you need to do the following:

1.  Download the binaries from <http://code.google.com/p/go/downloads/list>.
2.  Open the package (possibly with `opt-Open` if the package hasn't been signed) and proceed with installation using the defaults.
3.  To test the installation, open the go folder in the **spikes** repo, and run the **hello.go** sample by issuing

        $ go run hello.go

4.  Install the **GoSublime** package on Sublime Text 2. Instructions are available at <https://github.com/DisposaBoy/GoSublime#installation>.

5.  Make sure **GoSublime** is installed with all package dependencies:
    1.  Open **Preferences | Package Settings | GoSublime | Settings - User**
    2.  Make sure the **GOPATH** and **GOROOT** environment variables are properly set. Typically, the entries look like the following:

            {
				"env": {
					"GOPATH": "$HOME/Documents/projects/misc/go",
        			"GOROOT": "/usr/local/go"
        		}
			}

	3.  Open **Tools | Command Palette**. In the **GoSublime** commands, execute **Install/Update MarGo and Gocode**.