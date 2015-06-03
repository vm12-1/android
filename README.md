VM12-1 LickMePop Rom by Team Nocturnal Download the source

Please read the VM12-1 building instructions before proceeding.

Initialize:

Create the build directory :

$ mkdir ~/dev 
$ mkdir ~/dev/vm12-1
$ cd ~/dev/vm12-1 Init core trees without any device/kernel/vendor :

$ repo init -u https://github.com/vm12-1/android.git -b vm12.1 

sync repo
$ repo sync 

Building
After the sync is finished, please read the instructions from the Android site on how to build.

$. build/envsetup.sh 
$ lunch
$ make bacon -j8 
You can also build (and see how long it took) for specific devices like this:

$. build/envsetup.sh time brunch vm12-1_hammerhead-user make -j4

Remember to make clobber every now and then!

