# Campaign Finder Website Tutotial

## Step 1 - Download and Install Ruby
Download and install the latest version of ruby either on Windows (https://rubyinstaller.org/downloads/), installing all the components suggested and verifying that **gem -v** and **ruby -v** are the most recent installed version. You can then run **gem install bundler jekyll** and verify that **jekyll -v** is the most recent version.

Or on Mac (), verify that the most recent ruby version is installed and then also run **gem install bundler jekyll** to get the most recent version of jekyll.

## Step 2 - Serving the Website
Go to the folder location on the command line and run **bundle exec jekyll serve** which will host the website on a localhost. Use the provided link to go through the website.

## POTENTIAL ERROR:
One potential error when trying to serve the jekyll website is with a **wdm** installation. The command that I found to work is **gem install wdm -- --with-cflags=-Wno-implicit-function-declaration**