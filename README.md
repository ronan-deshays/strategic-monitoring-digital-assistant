# Digital assistant for strategic monitoring
Based on Power Platform and Google Alerts, this assistant collects automaticaly articles from internet and enable user to sort detected article by relevance.

## Keywords

strategic monitoring ; business intelligence ; legal watch ; regulatory surveillance ; scientific monitoring

## Features

* Collects each day new articles from given RSS feeds (e.g. Google Alerts)
* Sort, rate and delete articles detected by the assistant
* Filter articles to only see articles not already rated

## Prerequisites

(1) "professional Microsoft account" means that the user account has a Microsoft 365 E3 licence or equivalent (see [Microsoft entreprise plans comparison](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans)), some educational or non profit plans may also work.

### For developper

A professional Microsoft account (1), which gives access to the following tools :
* Power Apps - [website](https://make.powerapps.com)
* Power Automate - [website](https://emea.flow.microsoft.com)
* Sharepoint Lists - [SharePoint website](https://www.microsoft.com/microsoft-365/sharepoint/collaboration)

A free Google account, which gives access to the following tools :
* Google Alerts - [website](https://www.google.com/alerts)

### For end user

A professional Microsoft account (1), which gives access to the following tools :
* Power Apps - [install](https://powerapps.microsoft.com/downloads/)

## Installation

### [optional] Google Alerts articles gatherer

1. create as many Google Alerts as needed
2. enable "generate RSS feed" option on each Google Alert

### Sharepoint List for RSS flows and articles

1. Download the latest release of "articles_sharepoint_list_canva.xlsx" [here](https://github.com/ronan-deshays/strategic-monitoring-digital-assistant/releases/latest/download/articles_sharepoint_list_canva.xlsx) and "RSS_feeds_sharepoint_list_canva.xlsx" [here](https://github.com/ronan-deshays/strategic-monitoring-digital-assistant/releases/latest/download/RSS_feeds_sharepoint_list_canva.xlsx) ;

**For each Excel File :**
2. Go to a sharepoint website > All Apps > Lists > New List > From Excel > Upload local file ;
Select one of the files that you previously downloaded.

3. For each column named "Raw [...] > Select "Multiline text" (because length of URL is sometimes bigger than 255 characters) ;
4. Create the list (configure it as you like).

### Power Automate RSS gatherer

1. Download the latest release of "rss_gatherer_power_automate_package.zip" [here](https://github.com/ronan-deshays/strategic-monitoring-digital-assistant/releases/latest/download/rss_gatherer_power_automate_package.zip) ;
2. Go to the Power Automate **Cloud** editor (not Power Automate Desktop) > My flows > Import > Import Package (Legacy) > Upload a .zip package file ;
Select the "rss_gatherer_power_automate_package.zip" file that you previously downloaded ;
[details missing]

### Power Apps articles viewer

1. Download the latest release of "user_interface_power_apps_package.zip" [here](https://github.com/ronan-deshays/strategic-monitoring-digital-assistant/releases/latest/download/user_interface_power_apps_package.zip) ;
2. Go to the Power Apps editor website > Apps > Import canvas app > Upload a .zip package file ;
Select the "user_interface_power_apps_package.zip" file that you previously downloaded ;
3. Go through configuration steps as you like > Click the "Import" button > Open and test your app in the Power Apps Studio ;
[details missing]