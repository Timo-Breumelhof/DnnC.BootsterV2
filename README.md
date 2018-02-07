# DnnC.BootsterV2
DnnBootster version 2

## Description

A free open source responsive skin\theme for Dnn (DotNetNuke) using Bootstrap 4.0.0.beta.

A demo of the theme/skin can be viewed by visiting [http://www.dnnbootster.com](http://www.dnnbootster.com "Official DnnBootster site")

## Warning : Install on Dnn 08.00.00
There is a small bug in this version of Dnn that will stop the menu showing.
To solve this is quite easy to do by following theses steps below:

Go to '/Portals/' folder of your Dnn install
In this folder you will find a file called 'web.config'
Open this file and search for the following 3 lines of html

`<host factoryType="System.Web.Mvc.MvcWebRazorHostFactory, System.Web.Mvc"/>`

`<add namespace="DotNetNuke.Web.Mvc.Helpers"/>`
`<add namespace="Dnn.Modules.DynamicContentViewer.Helpers"/>`

Change the lines above to this:

`<!--<host factoryType="System.Web.Mvc.MvcWebRazorHostFactory, System.Web.Mvc"/>-->`

`<!--<add namespace="DotNetNuke.Web.Mvc.Helpers"/>-->`
`<!--<add namespace="Dnn.Modules.DynamicContentViewer.Helpers"/>-->`

Save the file and the menu's should display correctly.

## Theme Requirements & installation
Install the skin as you would with any other Dnn extension by going to the Host > Extensions page (you should not install via Admin/Extensions).
The Dnn Bootster them was created for Dnn8 and upwards.

To install follow the steps below:

1. Download and un-block the zip file from here.
2. Go to Host –> Extensions –> Install Extension wizard to install the Bootster skin pack.
3. After the installation has been completed, navigate to Admin –> Site Settings –> Basic Settings (tab) –> Appearance (section) and specify portal and edit skins and containers.

## Theme Configuration ##

### Changing Themes ###
To change the color theme of the skin is easy to do...
Open the skin.ascx and Home.ascx files found in the root of the skin folder 'Bootster'. At the top of the file look for a line with the ID of 'DnnCssThemeInclude' like below:

`<!-- Theme Css File --><dnn:DnnCssInclude ID="DnnCssThemeInclude" runat="server" FilePath="assets/themes/grey.css" PathNameAlias="SkinPath" /><!-- Theme Css File -->`


Enjoy!
