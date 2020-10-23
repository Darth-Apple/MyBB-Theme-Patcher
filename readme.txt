This plugin attempts to resolve "authorization mismatch errors" that exist in a number of older themes for MyBB. These fixes are necessary if you are unable to log in to your forum after updating to 1.8.16 (or after installing an older theme). These patches will be applied automatically upon activation and should resolve these issues on most themes!

Please keep in mind that this plugin cannot patch other theme issues unrelated to login-related problems. Any further updates/fixes will need to be made manually. However, this provides a best-faith effort to resolve issues that prevent users from logging on to your forum. This should resolve most such errors successfully. :)


*** Note that you DO NOT need to run this plugin on any theme that was developed for a MyBB version of 1.8.16 or newer. These themes are already patched.


--------------------------------------
   INSTALLATION INSTRUCTIONS 
--------------------------------------

IMPORTANT: We recommend making a backup of your forum database (or exporting your theme as a backup) before running this plugin. These patches cannot be reversed! 

To install/Patch: 

 - Upload the contents of the "Upload" directory to your MyBB forum root directory. 
 - Go to ACP -> Plugins and activate "MyBB Theme Patcher" 
 - Congratulations! All themes have been patched. You may now deactivate this plugin.  


--------------------------------------
  INSTALLING NEW THEMES 
--------------------------------------

 - Each time this plugin is run, it will fix all existing themes on your MyBB install (as needed). However, it cannot patch future themes unless the patch is run again. If you install a new theme that has not been updated for MyBB 1.8.16 (or newer), simply deactivate and reactivate this plugin to patch again. 

--------------------------------------
   UNINSTALLATION INSTRUCTIONS 
--------------------------------------

 - You may simply de-activate the plugin once the patches are completed. The patches will remain in place. 


----------------------------
 TROUBLESHOOTING: 
----------------------------

 - If your themes still display "authorization mismatch errors" after running this plugin, you will need to patch your themes manually. This may occasionally occur on certain highly modified themes if this plugin is unable to make sense of your theme's login-related templates. If this occurs, see this post for more information on how to fix your theme! https://community.mybb.com/thread-218862.html

 - Patches will remain in place following routine MyBB updates. However, master templates may occasionally be reverted if a specific template was updated on a new release of MyBB. If authorization mismatch errors re-occur, simply de-activate and re-activate this plugin to re-run the script as needed.


--------------------------------------
   SOME USEFUL INFO 
--------------------------------------  

 - This plugin works by detecting whether the required "{$mybb->post_code}" field exists in four templates: error_nopermission, header_welcomeblock_guest, member_login, and portal_welcome_guesttext. If this variable is not found, it automatically adds this field above the form's opening tag in order to patch the templates as necessary. 

 - This plugin will automatically detect any theme that has already been patched (whether manually or by the developer). It will safely skip any theme that does not require patches. You may safely run this plugin as many times as needed! 

 - Kindly translated to German by @tc4me at https://autism4all.at - This plugin includes both German and English language packs, no external language pack is necessary! 

	 
Licence & Copyright: 

 - You may port this plugin to future MyBB releases and redistribute as needed (according to the terms of the GPL v3 license). If you distribute a forked or modified version, my only request is that you leave credit and a link back to the original! :)


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
