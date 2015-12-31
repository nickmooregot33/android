Activity
---
- each screen is a custom subclass of an Activity
  - subclass defines behavior of activity
  - responsible for loading user interface from XML layout file

XML Layout File
---
- where the entire interface for a given activity is defined
- to display text fields, buttons, images, and widgets, just add XML elements to the layout file.

Intent Objects
---
- used to switch between various activities composing the app
- examples:
  - click a button to navigate to another screen
    1. create an intent object and pass the destination activity to it
    2. execute the intent to tell android to switch to the next page
  - The above is the general pattern for building up a multi-screen application
 
  
App Structure Overview
===
- **AndroidManifest.xml**
  - declares everything about your app the OS needs to launch it and includes:
    - classes composing the app
    - permissions required by the app
    - meta information like minimum android api for the app
    - libraries the app depends on\
  - must be in root directory of the project
  - typically the SDK updates this file automatically so no manual edits
- src/
  - contains all of the app's source files (java code)
- res/
  - contains application resources
    - images
    - videos
    - strings to be displayed
