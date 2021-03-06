---
license: >
    Licensed to the Apache Software Foundation (ASF) under one
    or more contributor license agreements.  See the NOTICE file
    distributed with this work for additional information
    regarding copyright ownership.  The ASF licenses this file
    to you under the Apache License, Version 2.0 (the
    "License"); you may not use this file except in compliance
    with the License.  You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing,
    software distributed under the License is distributed on an
    "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.

title: Project Settings for iOS
---

[Project Settings](../index.html) for iOS
========================

The `config.xml` settings file controls various settings of Cordova. This is application wide, and not set per CDVViewController instance.
The `config.xml` file is located in your `<project folder>/<appname>` directory.

Various preferences (as **&lt;preference&gt;** tags) default on not breaking existing apps. The available preferences are:

1. **UIWebViewBounce (boolean, defaults to true)** - set to false if you don't want the WebView to rubber-band

2. **TopActivityIndicator (string, defaults to 'gray')** - this is the top spinning throbber in the status/battery bar, valid values are "whiteLarge", "white" and "gray"

3. **EnableLocation (boolean, defaults to false)** - set to true, to initialize the [Geolocation](../../../cordova/geolocation/geolocation.html) plugin at start-up (so the fix on your location can be more accurate)

4. **EnableViewportScale (boolean, defaults to false)** - set to true to prevent viewport scaling through a meta tag

5. **AutoHideSplashScreen (boolean, defaults to true)** - set to false to control when the splashscreen is hidden through a JavaScript API

6. **ShowSplashScreenSpinner (boolean, defaults to true)** - set to false to [hide](../../../cordova/splashscreen/splashscreen.hide.html) the splash-screen spinner

7. **MediaPlaybackRequiresUserAction (boolean, defaults to false)** - set to true to not allow autoplayed HTML5 video

8. **AllowInlineMediaPlayback (boolean, defaults to false)** - set to true to allow inline HTML5 media playback, also, the video element in the HTML document must also include the webkit-playsinline attribute

9. **BackupWebStorage (string, defaults to 'cloud')** - valid values are 'none', 'cloud' and 'local'. Set to 'cloud' to allow the web storage data to be backed up to iCloud, and set to 'local' to only allow local backups (iTunes sync). Set to 'none' to not allow any backups of web storage.
	
10. **KeyboardDisplayRequiresUserAction (boolean, defaults to true)** - set to false to open the keyboard when form elements get focus via the JavaScript focus() call.

11. **SuppressesIncrementalRendering (boolean, defaults to false)** - set to true to wait until all new view content has been received before it is rendered.
