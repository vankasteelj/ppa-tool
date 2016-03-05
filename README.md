ppa-tool
========

Script to help handling PPA's through command line.
	
	Available options:
	 -h, --help	Print this help
	 -c, --check	Check the [PPA] compatibility with the system
	 -a, --add	Add [PPA] to repositories (implies -c, --check)
	 -r, --remove	Remove [PPA] from repositories
	 -p, --purge	Purge [PPA] and all installed packages coming from there
	 -l, --list	Get a list of all installed PPA's
	 -v, --version	Print the script's version number
	 --update	Update 'ppa-tool' to the most recent version
	
	Advanced options: BACKUP
	 --bkp-list	Make a backup of all installed PPA's in HOME
	
	 --bkp-install	Restore PPA from [FILE]
	
	Advanced options: CHECK
	 --chk-release=[VERSION]	Check the installed PPA's for an upgrade to [VERSION]
		=> All installed PPA's will be checked.
	
	 --chk-release=[VERSION]... [PPA]...	Check [PPA] compatibility with [VERSION]
		=> A fake check : is [PPA] compatible with [VERSION] ? 


###### INSTALLATION ######

To fetch the script in your language (if available) and install it in the right location :

	wget https://raw.githubusercontent.com/vankasteelj/ppa-tool/master/dist-install
	bash dist-install
	rm dist-install
	
To install from a cloned repo :

	git clone https://github.com/vankasteelj/ppa-tool.git
	cd ppa-tool
	bash install
	rm -r ../ppa-tool
