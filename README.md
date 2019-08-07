# AndroidDarkLightTheme

![Alt Text](https://media.giphy.com/media/S5DV7lASRNNUdzM8Cm/giphy.gif)


With the Arrival of the new version 23.2 of library support Android brings a new components that can enrich the user interface. There’s a new theme added to AppCompat in this release: Theme.AppCompat.DayNight.
Before adding this theme to AppCompact developers have to make adjustments to their designs to account for different ambient light levels or time of day, but AppCompat is now offering to automate a little bit of that. 
Based on your last known location, the latest version can switch between regular and “night” themes for apps.This means developers now have to maintain two sets of themes, but it should also make it better for users.

### Update colors.xml 
Add the below color values to the colors.xml located in res => values => colors.xml and res => values-night => colors.xml.
colors.xml file in values(for default mode) folder
    
        <?xml version="1.0" encoding="utf-8"?>
        <resources>
           <color name="colorPrimary">#3F51B5</color>
           <color name="colorPrimaryDark">#303F9F</color>
           <color name="colorAccent">#FF4081</color>
           <color name="textColorPrimary">#000000</color>
           <color name="colorBackground">#FFFFFF</color>
       </resources>
       
### colors.xml file in values-night(for night mode) folder
        <?xml version="1.0" encoding="utf-8"?>
        <resources>
           <color name="colorPrimary">#3F51B5</color>
           <color name="colorPrimaryDark">#303F9F</color>
           <color name="colorAccent">#FF4081</color>
           <color name="textColorPrimary">#FFFFFF</color>
           <color name="colorBackground">#000000</color>
        </resources>

### In your acctivity change Theme like below,
         AppCompatDelegate.setDefaultNightMode(AppCompatDelegate.MODE_NIGHT_NO);
         
         
Happie Coding:)         

