# Simple dashboard/slideshow for tv screens at jubii

## Description

A simple slideshow that shows random fading images at 1920x1080 resolution from https://source.unsplash.com/. The image fades out and reloads every 5 minutes.

## Usage

Go to url: https://jubii.github.io/dashboard/

Use the following querystring parameters to configure the page:

Param | Name | Format | Default
-|-|-|-
sz|size|*{number}x{number}*|*screen size*
t|timeout|*number between 30 and 86400 seconds*|300
f|featured|*0* or *1*|1
cat|category|buildings,food,nature,people,technology,objects|*not set*
col|collection|*collection id from unsplash*|*not set*
q|search terms|*{term1}[,{term2}...]*|*not set*

## Example urls

Default settings:
    https://jubii.github.io/dashboard/

Slide every 60 seconds from the buildings category
    https://jubii.github.io/dashboard/?t=60&cat=buildings

## Example windows shortcut

To startup a chrome instace on a machine at power-on use something like the following:

    "[path to chrome]\chrome.exe" --start-fullscreen --new-window https://jubii.github.io/dashboard/ --window-position=0,0
