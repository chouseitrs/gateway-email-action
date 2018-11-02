Email scripts for Gateway 2
-----------------------------------

**Introduction**

This solution is provides several different perl script to for use with gateway2.

**scripts**

The scripts directory contains the available email scripts.
email.pl
 Attempt at one stop shopping for multiple formats as opposed to having to maintain multiple scripts. Works for gateway user assignment and escalation. Accepts email addreses as either the userdata "eMail" or command line arguments. Makes subject nice and short so suitable for smartphones.

 Symlinking this script to the following names helps invoke different functionality:

* email_assign.pl -> email.pl
* email_unassign.pl -> email.pl
* email_escalate.pl -> email.pl

email_ws.pl
 Modification of email.pl to send dataviews as retrieved from webslinger to be sent as part of the email. Uses wget to access webslinger. As the webslinger URL is built using a static URL path you have to modify two lines at the top of the script.

* webslingerHost = the host: port of the webslinger url
* attributes = .Comma separated list of the attributes used by webslinger. Should match the webslinger.setup VIEW_PATH.

 Symlinking this script to the following names helps invoke different functionality:

* email_assign.pl -> email.pl
* email_unassign.pl -> email.pl
* email_escalate.pl -> email.pl