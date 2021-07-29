REMOVING ALL THE BLOATWARE (preinstall au apps) on LGT32 Qua tab PZ 

#To Factory reset
turn off device

press power & volume - together
keep holding volume - 
release power button once briefly and press power button again 

imp :volume - keep pressing
 
 Note
 To Force Restart (if stucked on android logo)
 press power & volume - together   until screen goes off (power off)
 Power button to start your device
 
 if still stuck on android screen
 
Step 1: Press and hold the Volume down button, Home button, and power button all at the same time.
Step 2: When you see the Android icon, release the power button, but keep holding the other two buttons until the recovery screen appears.
Step 3: Use the volume buttons to highlight the "Wipe Cache Partition" option and press the power button to initiate the process.
 
 if it fails
 FACTORY RESET
_______________________________________

#DEVELOPER MODE
settings> about> software info> Build Number  tap 7 times
developer mode > usb debugging on
select USB configuration > PTP

connect USB 
allow 


_____________________________________


# ADB Setup
download [adb fast boot](https://forum.xda-developers.com/showthread.php?t=2317790) 

extract the file
inside folder right click 
open powershell or command
 
 type 
 adb shell  
 if doesnot work
 type
 ./adb shell  
 
 ___________________________________________________
 
 # list packages A
 then 
 To list all the installed packages on an Android device
  pm list packages
 To list only 3rd party (or non-system) packages, use the “-3” option.
 pm list packages -3

To list only the system packages, use the “-s” option.
 pm list packages -s
 
 To list the package names as well as the path to the installed APK files, use the “-f” option.
 pm list packages -f
 
 # list packages B
 dowload the app Package Name Viewer    - it will show the apk package name
 https://play.google.com/store/apps/details?id=com.csdroid.pkg&hl=en_US&gl=US
 
 install it 
 
 if cannot download form play store 
 open apkpure.com
 paste the above link in apkpure 
 
 download
 move downloaded apk file to the adb folder 
 then install using adb
 
 
 _______________________________________________
 # install Packages ADB
 to install via adb
  move the file to the same folder where you are running the adb from then
  
 ./adb install apkname.apk
 
 
 
 # delete  bloatware
 now copy APKPACKAGENAME  you want to uninstall, 
 pm uninstall --user 0 .com*PACKAGENAME
 
 
# Delete Au Apps

pm uninstall --user 0 com.kddi.android.lismobookstore
pm uninstall --user 0 com.kddi.android.smartpass
pm uninstall --user 0 com.kddi.disasterapp
pm uninstall --user 0 com.kddi.auoneshopping
pm uninstall --user 0 com.kddi.android.UtaPass
pm uninstall --user 0 com.kddi.android.mieruka
pm uninstall --user 0 com.kddi.android.auhomelauncher
pm uninstall --user 0 com.kddi.cs.app001
pm uninstall --user 0 com.kddi.android.klop
pm uninstall --user 0 com.kddi.android.aumanagementsystem
pm uninstall --user 0 com.kddi.android.au_wifi_connect2
pm uninstall --user 0 com.kddi.pass.launcher
pm uninstall --user 0 com.kddi.datacharge
pm uninstall --user 0 com.uievolution.gguide.android
pm uninstall --user 0 com.kddi.android.repairreceipt
pm uninstall --user 0 com.kddi.android.checker_android
pm uninstall --user 0 com.kddi.market
pm uninstall --user 0 com.kddi.ux.station
pm uninstall --user 0 com.kddi.android.au_setting_menu
pm uninstall --user 0 com.kddi.android.easysettingwizard
pm uninstall --user 0 com.kddi.android.auoneidsetting
pm uninstall --user 0 com.kddi.android.ausharelink
pm uninstall --user 0 com.kddi.android.kddigallery
pm uninstall --user 0 com.kddi.android.mamoru
pm uninstall --user 0 com.kddiandroid.email
pm uninstall --user 0 com.kddi.emailprov
pm uninstall --user 0 com.kddi.android.imp
pm uninstall --user 0 com.real.RealPlayerCloud
pm uninstall --user 0 com.kddi.ar.satch.satchviewer
pm uninstall --user 0 jp.co.optim.oru
pm uninstall --user 0 jp.auone.wallet
pm uninstall --user 0 web.wm.auone.jp
pm uninstall --user 0 jp.netstar.familysmile
pm uninstall --user 0 jp.co.ise.lgt32.instructionmanual
pm uninstall --user 0 jp.co.omronsoft.iwnnime.ml


# Delete info clock
pm uninstall --user 0 com.lge.srw

 # Delete Facebook

pm uninstall --user 0 com.facebook.katana
pm uninstall --user 0 com.facebook.system
pm uninstall --user 0 com.facebook.appmanager
