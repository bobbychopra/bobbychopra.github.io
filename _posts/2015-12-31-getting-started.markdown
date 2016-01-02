---
layout: post
title:  "Getting started is never that simple"
date:   2015-12-31 22:00:00 -0500
categories: jekyll blog 
---

I setup my [github page], which was quick & easy. Setting up [Jekyll with Pages on Windows] proved to be much more involved. I had to do the following:

* Install Ruby
  * Install [Chocolatey]
  * Open a Windows Powershell Command Prompt
  * Run the command `choco install ruby -y`
  * Close the Windows Powershell Command Prompt
* Install [Ruby DevKit]
  * Download an appropriate dev kit from [http://rubyinstaller.org/downloads/]
  * Extract it to some folder
  * Open a Windows Powershell Command Prompt
  * cd to that folder
  * Run the command `ruby dk.rb init`
  * Run the command `ruby dk.rb install`
  * Close the Windows Powershell Command Prompt
* Install the [Certificate for Ruby]
  * Download the cacert.pem file from http://curl.haxx.se/ca/cacert.pem
  * Save it to a permanent folder and set the environment variables `SSL_CERT_FILE` on this folder from the Control Panel
* Install the [Gems]
  * Open the Windows Powershell Command Prompt
  * Run the comand `gem update --system 2.3.0`
  * Run the command `gem install jekyll`
  * Close the Windows Powershell Command Prompt

_If you still fail, maybe you can try the step-by-step guide to setting up [Jekyll on Windows]_


That should make it all work. Phew!




[github page]:                  https://pages.github.com/
[Jekyll with Pages on Windows]: https://help.github.com/articles/using-jekyll-with-pages/
[Chocolatey]:                   https://chocolatey.org/
[Ruby DevKit]:                  http://jekyll-windows.juthilo.com/1-ruby-and-devkit/
[Gems]:                  https://github.com/imathis/octopress/wiki/Installation-Instructions-2.0-on-Windows
[Certificate for Ruby]:         https://gist.github.com/fnichol/867550
[Jekyll on Windows]:            http://jekyll-windows.juthilo.com/