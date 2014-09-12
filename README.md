If you wanna build OmniPlus, follow these steps:

1) Firstly create a new directory:
    mkdir omniplus
    
2) Init:
    repo init -u git://github.com/OmniPlus/android.git -b android-4.4
    
3) Download the source:
    repo sync
    
    
    
You downloaded the source. But you must download also device-specific things:

Type:
    source build/envsetup.sh
    
Download device sources of your device:
    breakfast maguro (hammerhead is codename of Galaxy Nexus. So on.)
    
Then download vendor blobs for your device:
    Open up https://github.com/DonkeyCoyote with your web browser. For example if you're gonna build for Galaxy Nexus, select proprietary_vendor_samsung repository, then make sure 4.4 branch is selected. Then hit download button. I'm assuming you're gonna build for Galaxy Nexus, so extract "maguro" folder to omniplus_folder/vendor/samsung/ directory. Of course there is no folder called "samsung" there, create that. I said "samsung" folder because manufacturer of Galaxy Nexus is Samsung, and so on.
    
Okay you downloaded everything needed, let's build:

Type:
    source build/envsetup.sh
    lunch maguro (just an example, maguro is Galaxy Nexus, put your device's codename there.)
    brunch maguro (just an example, again.)
