LineageOS 14.1 for Aristo 2
------------------------------------

Create directories

	$ mkdir cm-14.1
	$ cd cm-14.1

Init lineage:

	$ repo init -u git://github.com/LineageOS/android.git -b cm-14.1
  

Download and move the manifest xml for the device to .repo/local_manifests/

Then sync up with this command:

	$ repo sync --force-sync -q

-------------
 
_Building from source_
---------------

	$ . build/envsetup.sh
	$ lunch lineage_DEVICENAME-userdebug
	$ mka bacon
