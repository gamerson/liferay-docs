# Liferay Code Upgrade Tool

# Introduction

Liferay Code Upgrade Tool is available in Liferay IDE 3.1 or greater. This tutorial shows you how to use the tool to upgrade your liferay 6.2 plugin projects to liferay 7.0 plugin projects or liferay workspace.

Open Liferay Code Upgrade Tool: Project &rarr; Liferay Code Upgrade Tool...

# Welcome Page

Welcome to the Liferay code upgrade tool. This tool will helps you to upgrade Liferay 6.2 plugin projects into Liferay 7.0 projects. In this page, we will introduce some key functions, notes and show how to use it.

The initial 'Liferay Code Upgrade tool' looks like the belowing:

![welcome page](images/welcome.png)

## 1 The key funcitions

1. Convert Liferay Plugins SDK 6.2 to Liferay Plugins SDK 7.0 or to Liferay Workspace.

2. Update Descriptor files from 6.2 to 7.0.

3. Fink Breaking Changes in the APIs that need to be migrated to Liferay 7.

4. Build Service for your service-builder projects. Requires Java 8.

5. Update Layout Template files from 6.2 to 7.0 format.

6. Automatically Convert Custom JSP Hooks to OSGI modules.

7. Build all your projects.

8. Summary for upgrade results.

## 2 Buttons

1. ![restart upgrade button](images/restartUpgrade.png) : Click `Restart Upgrade` button to re-run liferay code upgrade tool.

2. ![show all pages button](images/showAllPages.png) : Click `Show All Pages` button to see all pages.

It will forward to 'Upgrade Descriptor Files' page automatically when clicking OK button in the popped up dialog after clicking on 'Show All Pages' button.

![show all code upgrade tool pages](images/allPages.png)

## 3 Attentions

1. It is highly recommended that you backup copies of your original plugin files before continuing.

2. Ext projects are not supported to upgrade in this tool currently.

For more details, please see [From Liferay 6 to Liferay 7](https://dev.liferay.com/develop/tutorials/-/knowledge_base/7-0/from-liferay-6-to-liferay-7).

## 4 What the button icons & symbols mean

`←` Go back to the previous page.

`√` Mark as resolved or completed.

`×` Mark as error or uncompleted.

`→` Go to next page.