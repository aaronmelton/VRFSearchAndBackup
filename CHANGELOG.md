# VRFSearchAndBackup.py #
---

## VRFSearchAndBackup v0.0.2-alpha (2013-08-22) ##
* Added whitespace to the end of the "show running-config | section SMVPN"
  command to prevent incorrect matches.  (Without the space at the end, a
  search for "3" would also return "31" or "300", etc.)

## VRFSearchAndBackup v0.0.1-alpha (2013-08-20) ##
* Initial commit.