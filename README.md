# ProCache StackPath
Purge the StackPath CDN cache when ProCache clears.

## Overview
If you use [StackPath's CDN](https://www.stackpath.com/products/cdn/) to deliver your website, you need a way to clear its cache when ProCache clears. This module connects with your StackPath stack via the StackPath API and when ProCache clears it requests StackPath clear the cache, attempting to respect the specific rules (Parents, Family, Children etc) set up in ProCache.

## Installation
1. Download the [zip file](https://github.com/nbcommunication/ProCacheStackPath/archive/master.zip) at Github or clone the repo into your `site/modules` directory.
2. If you downloaded the zip file, extract it in your `sites/modules` directory.
3. In your admin, go to Modules > Refresh, then Modules > New, then click on the Install button for this module.

**ProcessWire >= 3.0.210, ProCache >= 4.0.3 and PHP >= 8.1.0 are required to use this module.**

## Configuration
Once installed, log in to your StackPath account and navigate to API Credentials. Click *Generate Credentials* and enter a name, perhaps something like yourwebsitedomain.com:ProCacheStackPath. Click *Save*.

Copy the **Client ID** and **API Client Secret** to the module settings and click *Submit*. You should then be able to choose your stack from the **Stack** dropdown list.

You can now close the API details modal in your StackPath admin.

## License
This project is licensed under the Mozilla Public License Version 2.0.
