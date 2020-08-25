# Disable OneDrive Personal, Enable OneDrive Business
(from https://answers.microsoft.com/en-us/msoffice/forum/msoffice_onedrivefb-mso_o365app/how-to-turn-offhide-onedrive-personal-but-leave/bea35a10-78e9-4b35-a5df-c69060ad509b)

To disable the synchronizing of personal OneDrive accounts, you can use the User Configuration group policies for OneDrive. They can be found under User Configuration\Policies\Administrative Templates\OneDrive. For more detailed information, please refer to Administrative settings for the OneDrive for Business Next Generation Sync Client.

To remove the OneDrive-personal icon on File Explorer, you can try the steps below:

Note: It only works when you already have OneDrive-personal icon appear on File Explorer.

Press windows key+R to open Run dialog box.
Type regedit.exe then press enter to open registry editor.
Go to the following location:
hkey_current_user\software\microsoft\windows\currentversion\explorer\desktop\namespace
Find the subkey for OneDrive personal. Usually, it is {018D5C66-4533-4307-9B53-224DE2ED1FE6}. But it is OK if different.
Go to the following location: hkey_classes_root\clsid
Find the key that matches OneDrive personal which you find in step 4.
In the subkey system.ispinnedtonamespacetree change the value date from 1 to 0.
Save the change.
 

Note: Before you modify the registry, back up the registry for restoration  in case problems occur. 

WARNING: Using Registry Editor incorrectly can cause serious problems that may require you to reinstall your operating system. Microsoft cannot guarantee that problems resulting from the incorrect use of Registry Editor can be solved. Use Registry Edit at your own risk.
