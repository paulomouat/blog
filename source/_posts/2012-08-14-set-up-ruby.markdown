---
layout: post
title: "Set up Ruby, RVM, Rails and the blog"
date: 2012-08-14 21:03
comments: true
categories: Dev
---

To install the Ruby-related tools:

Install RVM, Ruby 1.9.3 and Rails 3 by following the directions at <http://pragmaticstudio.com/blog/2010/9/23/install-rails-ruby-mac/>

Then, to set the blog up, run the following on the command-line:

    cd blog
    gem install bundler
    bundle install
    rake setup_github_pages