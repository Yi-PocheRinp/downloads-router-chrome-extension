Downloads Router
===============

Downloads Router is an extension for Chromium and Google Chrome that allows the user
to establish routing rules, directing downloads to folders based on filetype, filename, or source domain.

* [Chrome web store listing][webstore]

[webstore]: https://chrome.google.com/webstore/detail/downloads-router/fgkboeogiiklpklnjgdiaghaiehcknjo


Changelog
---------

### 0.8.1 (September 30, 2014)

* Referrer downloads now use URL as fallback if no referrer information is provided
* Now correctly marks the mime-type of torrent files sent as octet-streams, permitting MIME routing from sources such as torcache
* Provided fallback setting in case no rule order has been saved, a case that previously broke the extension

### 0.8 (August 27, 2014)

* Added the global referrers folder mapping option
* Tweaked the ``fresh install'' detection mechanism to trigger on updates as well

### 0.7 (July 26, 2014)

* Custom ruleset order added
* Tweaked referrer-based routing behavior to exclude the www subdomain
* Improved usage instructions and removed erroneous (outdated) information

### 0.6 (April 14, 2014)

* Filename-based routing option added
* Update usage instructions
* Streamlined map unpacking and table code generation in options.js

### 0.5 (March 03, 2014)

* Tabbed interface for the configuration page
* Very rudimentary trailing character check implemented

### 0.4 (February 20, 2014)

* Implemented a basic workaround for downloads sent as `application/octet-stream`
* Updated usage instructions with more accurate information regarding usage on OSX
* Added a troubleshooting section on the options page

### 0.3 (February 18, 2014)

* Automatically opens the options page directly after installing
* Added locale support and very rudimentary translations for Swedish and Spanish; options page i18n pending

### 0.2 (February 17, 2014)

* Tested on Windows, updated information in Options to reflect findings

### 0.1 (February 17, 2014)

* Initial commit, tested on Linux (Chromium) and OS X (Google Chrome)
* Options page allows the creation of routing rules based on filetypes and referrer
* The manager listens to `onDeterminingFilename` events and creates suggestions based on the maps created on the options page
