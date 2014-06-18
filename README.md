JCROM on AOKP
====================================


Download the Source
===================

Please read the [AOSP building instructions](http://source.android.com/source/index.html) before proceeding.

Initializing Repository
-----------------------

Init repo with all devices, kernels and vendors supported by AOKP :

    $ repo init -u https://github.com/JCROM-Android/aokp_platform_manifest.git -b kitkat-jcrom -g all,kernel,device,vendor

sync repo :

    $ repo sync

***

Building
--------

After the sync is finished, please read the [instructions from the Android site](http://s.android.com/source/building.html) on how to build.

    . build/envsetup.sh
    brunch


You can also build (and see how long it took) for specific devices like this:

    . build/envsetup.sh
    time brunch aokp_hammerhead-userdebug

Remember to `make clobber` every now and then!
