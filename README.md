# Light Blur Skin
Custom skin for Home Assistant HADashboard 2 that looks a little like the iOS Home app. 

![alt tag](/blur-theme-light.png)

Note that dashboard.css and variables.yaml alone won't make your dashboard look like the screenshot, you must also modify your dashboard files.  In order to gain more control over the exact size and position of dashboard elements I am using widget dimensions of 1x1 pixels.

Below is a snippet of my dashboard file. Notice that since widgets now have a dimension of 1x1 pixels you will need to create a widget that is 120x120 widgets to replicate a "normal" 120x120 pixel widget. This also means that you need as many empty rows as you want pixels between widgets and spacers equal to the number of pixels you want between columns.

```
layout:
    - empty: 120
    - spacer(20x1), media(120x120)
    - empty: 140
```
