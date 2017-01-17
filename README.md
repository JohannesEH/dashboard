# Simple dashboard/slideshow for tv screens at jubii

## Description

A simple slideshow that shows random fading images at 1920x1080 resolution from https://source.unsplash.com/. The image fades out and reloads every 5 minutes.

## Usage

Go to url: https://jubii.github.io/dashboard/

Use the following querystring parameters to configure the page:

<table>
    <thead>
        <tr>
            <td>Param</td>
            <td>Name</td>
            <td>Format</td>
            <td>Param</td>
        </tr>
    </thead>
    <tbody>
        <tr><td>sz</td><td>size</td><td>*{number}x{number}*</td><td>*screen size*</td></tr>
        <tr><td>t</td><td>timeout</td><td>*number between 30 and 86400 seconds*</td><td>300</td></tr>
        <tr><td>f</td><td>featured</td><td>*0* or *1*</td><td>1</td></tr>
        <tr><td>cat</td><td>category</td><td>buildings,food,nature,people,technology,objects</td><td>*not set*</td></tr>
        <tr><td>col</td><td>collection</td><td>*collection id from unsplash*</td><td>*not set*</td></tr>
        <tr><td>q</td><td>search terms</td><td>*{term1}[,{term2}...]*</td><td>*not set*</td></tr>
    </tbody>
</table>

## Example urls

Default settings:
    https://jubii.github.io/dashboard/

Slide every 60 seconds from the buildings category
    https://jubii.github.io/dashboard/?t=60&cat=buildings

## Example windows shortcut

To startup a chrome instace on a machine at power-on use something like the following:

    "[path to chrome]\chrome.exe" --start-fullscreen --new-window https://jubii.github.io/dashboard/ --window-position=0,0
