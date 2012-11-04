SABnzbd epub to mobi script
=====

Post processing script to convert `epub` ebooks to `mobi` format. You can also send to your Kindle.

## Dependencies

* [SABnzbd](http://sabnzbd.org/) - Version 0.5.0 or greater
* [Python](http://www.python.org/getit/) - I only tested on 3.3
* [KindleGen](http://www.amazon.com/gp/feature.html?ie=UTF8&docId=1000765211) - Amazon's conversion tool
* Optional: [sendKindle](https://github.com/kparal/sendKindle) (or [my fork](https://github.com/sylturner/sendKindle) for Python 3.x) - only necessary if you want it to send to your Kindle.

## Setup

* Put the `KindleGen` binary in your SABnzbd [user scripts](http://wiki.sabnzbd.org/user-scripts) directory.
  * If using `sendKindle`, put the script in the user scripts directory.
  * Run `sendKindle` through command line once to create its config file.
  * Edit the config file with SMTP and Kindle settings.
* Configure SABnzbd to use the `epub-to-mobi.py` post processing script for ebooks