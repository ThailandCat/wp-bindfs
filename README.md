# wp-bindfs
Elegant way to use bindfs to correct permissions for WP site


In traditional development the problem with permissions arise in case developer want to access files on staging or testing environment. Usually web project run under some service account, for example www-data, which is also service account for webserver / php processor / etc.

So, if developer connect with his / her ssh credentials, then it may have problem to access / modify files which is run under service account.


To solve this problem, we will use bindfs and map website root dir to some dir under developer home account.

