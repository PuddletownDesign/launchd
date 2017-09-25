# Puddletown Launchd Jobs

Some quick launchd scripts to backup development configuration to github each hour if there are updates to push.

## Installation

1.  Clone/ Fork this repository or copy the com.puddletowndesign files into your `LaunchAgents` Directory. I've simply only added my own plist files into the repo while not adding any of the existing ones generated by apps.

2.  Edit the `com.puddletowndesign.backup.plist` & `com.puddletowndesign.update.plist` to match your username. (Change brent to your own username.)

3.  Clone/ Fork the <https://github.com/PuddletownDesign/bin> into `~/Dev/Config`

4.  Edit the `backup-configs.sh` file for the files that you have on your system. Delete all the sections for folders you don't have.

5.  Symlink the files to the LaunchAgents Directory


    ln -s ~/Dev/Config/LaunchAgents/com.puddletowndesign.backup.plist ~/Library/LaunchAgents/com.puddletowndesign.backup.plist

    ln -s ~/Dev/Config/LaunchAgents/com.puddletowndesign.update.plist ~/Library/LaunchAgents/com.puddletowndesign.update.plist

6.  Load the jobs into launchd

Done!
