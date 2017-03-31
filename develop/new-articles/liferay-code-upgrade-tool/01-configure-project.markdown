# Liferay Code Upgrade Tool

# Configure Project Page

This page will help you convert your *Liferay Plugins SDK 6.2* to *Liferay Plugins 7.0* or to *Liferay Workspace*.

The initial status looks like the following:

![initial status](images/initial.png)

## 1 Liferay Plugins SDK Location

This step you can click `Browse...` button to browse a correct sdk location for upgrading. Otherwise, it will show validation error.

![valid sdk location](images/correctSDKLocation.png)

![invalid sdk location](images/errorSDKLocation.png)

## 2 Select Migrate Layout

This step you can choose upgrade liferay plugins SDK 6.2 to liferay plugins 7.0 or to liferay worksapce. It has been set to 'Upgrade to Lifeary Workspace' by default.

![Select Migrate Layout](images/selectMigrateLayout.png)

## 3 Server Name

1) Upgrade to Liferay Plugins SDK7 

Liferay 7 portal bundle is required here. You can click `Add Server...` button to browse one.

![need to add server](images/addServer.png)

![Upgrade to Liferay Plugins SDK7](images/upgradeToSDK.png)

*Note: The most important thing is that you need to point to the correct `build.{username}.properties` file to pass the validation for sdk location.*

2) Upgrade to Liferay Workspace

It has the default `Liferay Server Name` and `Bundle Url` when upgrading to liferay workspace. You can also set other values. 

- Liferay Server Name: Default value is 'Liferay 7.x'.
- Bundle URL: Provides a default url to initiate a bundle for deploying projects.

![Upgrade to Liferay Workspace](images/upgradeToLW.png) 

## 4 Backup SDK into folder

Checked this checkbox will help you backup your original 6.2 sdk to your eclipse workspace. You can extract it and rerun code upgrade tool once you failed to import your projects.

## 5 Import Projects

1) Click `Import Projects` button to import your projects into eclipse workspace 
after the upper steps. It will forward to 'Update Descriptor Files' page automatically once finish importing.

![finished import projects](images/finishedImport.png)

2) You may not import projects successfully since the following reasons:

-  Haven't downloaded ivy caches completely.
-  Some internet problems. For example it needs internet to download a bundle from your bundle url during initiating a bundle. 

3) Workarounds when failed to import projects:

- You can click `Restart Upgrade` ![restart upgrade button](images/restartUpgrade.png) button in top right corner.
- You also can *Upgrade SDK 6.2 to SDK 7.0 manually or use blade cli to init liferay workspace in your SDK* and *import projects you want to upgrade into Eclipse workspace manually* then click `Show All Pages` ![show all pages button](images/showAllPages.png) button next to `Restart Upgrade` button in top right corner.
