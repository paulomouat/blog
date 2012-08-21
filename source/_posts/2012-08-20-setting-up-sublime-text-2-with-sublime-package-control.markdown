---
layout: post
title: "Setting up Sublime Text 2 with Sublime Package Control"
date: 2012-08-20 21:13
comments: true
categories: [Setup, Sublime Text]
---

Install **Sublime Package Control** from <http://wbond.net/sublime_packages/package_control> by doing the following (if you run into any issues, there are additional details at <http://wbond.net/sublime_packages/package_control/installation>):

1.  Run the following command from the Sublime Text console, invoked through ``Ctrl+` `` (this is a long single line of code, you will have to scroll right to see it in full):

        import urllib2,os; pf='Package Control.sublime-package'; ipp=sublime.installed_packages_path(); os.makedirs(ipp) if not os.path.exists(ipp) else None; urllib2.install_opener(urllib2.build_opener(urllib2.ProxyHandler())); open(os.path.join(ipp,pf),'wb').write(urllib2.urlopen('http://sublime.wbond.net/'+pf.replace(' ','%20')).read()); print 'Please restart Sublime Text to finish installation'

2.  Restart Sublime Text.