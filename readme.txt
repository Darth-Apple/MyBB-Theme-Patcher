Thank you for downloading MyBB Theme Patcher! 

WARNING: THIS IS PRE-RELEASE! PLEASE MAKE A BACKUP OF YOUR FORUM BEFORE USE!!

This plugin resolves "authorization mismatch errors" that exist in a number of older themes for MyBB. Most themes designed for MyBB 1.8.16 or below will require certain fixes in order to function as intended. Without these fixes, users will be unable to log onto your forum. This plugin applies these patches automatically and performs all necessary template edits (simply upload and activate)! 

Please keep in mind that this plugin ONLY fixes authorization mismatch errors. Older themes may have additional bugs or issues that cannot be fixed by this plugin. Likewise, this plugin is not guaranteed to work on every single theme. It is simply a best faith effort to patch as many old themes as possible! :) 

Note: This plugin is only necessary for themes shipped for MyBB 1.8.16 and below. It will safely skip any themes that have already been updated or that don't need patches. 

--------------------------------------
   INSTALLATION INSTRUCTIONS 
--------------------------------------

IMPORTANT: Make a backup of your database before running this plugin! These patches cannot be reversed. 

To install/Patch: 

 - Upload the contents of the "Upload" directory to your MyBB forum root directory. 
 - Go to ACP -> Plugins and activate "MyBB Theme Patcher" 
 - Congratulations! All themes have been patched. 

 - You may now de-activate the plugin. Patches will remain in place. 


--------------------------------------
  INSTALLING NEW THEMES 
--------------------------------------

 - Each time this plugin is run, it will fix all existing themes on your MyBB install (as needed). If you install a new theme that has not been updated for MyBB 1.8.16 (or newer), you must run the theme patcher again. Simply de-activate and re-activate the plugin to patch any newly installed theme. 


--------------------------------------
   UNINSTALLATION INSTRUCTIONS 
--------------------------------------

 - You may simply de-activate the plugin once the patches are completed. The patches will remain in place even after the plugin has been de-activated. 


----------------------------
 TROUBLESHOOTING: 
----------------------------

 - If your themes still display "authorization mismatch errors" after running this plugin, you will need to patch your themes manually. See this post for more information: https://community.mybb.com/thread-218862.html

 - Patches will remain in place following routine MyBB updates. However, occasionally master templates may be reverted if a specific template was updated on a new release of MyBB. If authorization mismatch errors re-occur, simply de-activate and re-activate this plugin to re-run the script as needed.


--------------------------------------
   SOME USEFUL INFO 
--------------------------------------  

 - This plugin automatically detects themes that have already been patched (whether by the developer, manually, or by this plugin). You may safely run this plugin as many times as needed. It will skip over any theme that has already been patched already (even if the theme was patched manually). 

 - This plugin will also leave any newer (MyBB 1.8.17+) themes completely untouched. It detects these automatically and does not modify them. 

 - This plugin has been developed by us over at http://makestation.net. We develop a number of other plugins as well. Feel free to check us out! We're always happy when users discover our plugins and find them useful on their communities. :)


	 
Licence & Copyright: 

 /*     This file is part of Theme Patcher
  
    Theme Patcher is free software: you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
    (at your option) any later version.

    Theme Patcher is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with Theme Patcher.  If not, see <http://www.gnu.org/licenses/>. */
