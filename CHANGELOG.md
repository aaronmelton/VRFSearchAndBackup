# VRFSearchAndBackup.py #
---

## VRFSearchAndBackup v0.0.5-alpha (2013-08-29) ##
* Updated the backupVRF function so that the application will not log into
  any routers and retrieve results if the output file cannot be opened.
* Corrected 'mkdir' function to 'makedirs' so that directories will be
  created recursively, if they do not exist.
* Added basic logging to file to track results if application has to connect
  to a router to run buildIndex().
* Suppressed error SPAM from stdout by adding stderr=(open(os.devnull, 'w'))
  to the Queue() function. (Errors are still written to the log.)

## VRFSearchAndBackup v0.0.4-alpha (2013-08-28) ##
* Added functionality to specify configFile from the command line.
* Updated README.md

## VRFSearchAndBackup v0.0.3-alpha (2013-08-26) ##
* Created README.md, VRFSearchAndBackup.png
* Updated TODO.md, code comments to reflect current functionality.  
* Removed unused modules.

## VRFSearchAndBackup v0.0.2-alpha (2013-08-22) ##
* Added whitespace to the end of the "show running-config | section SMVPN"
  command to prevent incorrect matches.  (Without the space at the end, a
  search for "3" would also return "31" or "300", etc.)

## VRFSearchAndBackup v0.0.1-alpha (2013-08-20) ##
* Initial commit.