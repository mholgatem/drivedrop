# DriveDrop
Create an embeddable form that can be used to allow anyone to upload files to your Google Drive
<img style="width:45%;margin:5px" src=https://github.com/mholgatem/drivedrop/raw/master/images/form.jpg>

You can create a copy of DriveDrop by clicking below
## [- Click Here To Clone DriveDrop -](https://script.google.com/d/1mA2_OMh2Fdt9qTg2MYr5NIy_QtYbE_wAtecHt8NgBvtWC5lVCBT-sSha/edit?newcopy=true)

## Instructions
1. Clone the code
2. Select 'Publish → Deploy as web app'
3. Set 'Execute the app as: Me'
4. Set 'Who has access to the app: Anyone, even anonymous'
5. Click 'Update'

From here you will get a prompt that says
```
Authorization required

DriveDrop by mholgatem (Master) needs your permission to access your data on Google.
```
1. Click 'Review Permissions'
2. Select the account that you want files to upload to
3. You will get a scary looking warning because you have not submitted this app to be verified by Google 
4. Click advanced
<img src=https://github.com/mholgatem/drivedrop/raw/master/images/warning.jpg>

5. Click 'Go to DriveDrop by mholgatem (Master) (unsafe)'
6. This will show you the consent screen, review the permissions, then click 'Allow'
<img src=https://github.com/mholgatem/drivedrop/raw/master/images/consent.jpg>

Congratulations! Your form is now live! Anyone with the link can now upload files to your Google drive!

If you want to embed your new form, you need to make a few changes to the code:
1. Open server.gs
2. Find the Config section for the picker
```
  PICKER :
  {
    embedded : false, //set to true if you want to embed in an Iframe
    URL      : "https://script.google.com", // default URL
    embedURL : "http://your.website.com" // URL to use if embedded
  }
```
3. set embedded to 'true'
4. set embedURL to the URL of your site

