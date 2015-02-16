# VRFSearchAndBackup.py #
---

## VRFSearchAndBackup v1.0.3 (2015-02-16) ##
* Corrected Issue #1 https://github.com/aaronmelton/VRFSearchAndBackup/issues/1
* Changed "vrfName = word[0]" to "vrfName = word[0].strip()" to correctly
  strip white space from this variable.

## VRFSearchAndBackup v1.0.2 (2014-03-24) ##
* Changed text "Enter the VRF Name or IP Address you are searching for" to
  "Enter the VRF Name or Peer IP Address you are searching for" to clarify
  which IP the user should be entering.

## VRFSearchAndBackup v1.0.1 (2014-03-17) ##
* Replaced tab with four spaces.
* Replaced ' with " to be consistent throughout the file.
* Corrected problem where application would fail if logFileDirectory or 
  backupFileDirectory in settings.cfg was blank.

## VRFSearchAndBackup v1.0.0 (2013-11-13) ##
* Added functionality to strip whitespace from user input
* Application has been functioning without major issues since last release;
  pushing to "production" status.

## VRFSearchAndBackup v0.0.6-alpha (2013-09-09) ##
* Corrected makedirs() functionality: Directories with a trailing backslash
  in the config file were not being created thereby causing the application
  to fail.
* Moved logFileDirectory & backupDirectory makedirs() function such that the
  directory would only be created if/when the parent function was called
  instead of creating both directories whenever the application executed.
* Removed 'dated' variable, which was a duplicate of global variable 'date'

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