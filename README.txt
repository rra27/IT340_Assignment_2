Since core nagios does not natively support MySQL monitoring without external plugings (which last time I said were utterly useless) I opted to use Nagios XI for this project since it was far more comprehensive with it's use. Setting up most of the functions was rather easy though disk quotas were much more difficult. 

This I attribute to most of the guides and such requiring you to use usrquota permissions on the /home partition though I have none set on my system, as showm in the provided fstab file. I did however attempt to give usrquota permissions to the other noted directories without success. When attempting to remount the partition it also would stop working and I would have to restore to a previous snapshot

One thing I noted was that when installing Nagios XI, it was  incompatible with the core nagios npre install and I had to remove it before proceeding. Likely it was not designed for the configuration wizards utilized in nagios xi.
