# Custom Page Settings


### Summary

* purpose is to provide custom specific settings to less than admins

* open architecture, can be extend through config files and/or custom assemblies

* settings can be of different types (Boolean, texts, etc.)

* settings can be inherited from host scope to portal scope to page scope

* settings can be locked for modification at any level

* settings can be accessed from: 

    Header template
    <br />
    HttpContext.Items (todo)
    <br />
    My Tokens (todo)
    <br />
    Building Block (todo)
    
<br />
The Settings engine allows administrators to control the content of the website/page. It is an open engine - in Config there's a .json file in PageVars that has all the existing settings defined (for example, TwitterId, FacebookId, LinkedInId) and each one of them has some settings like Title, Type etc. If you want to change the field type, you can replace the default "text" type with the "textarea" type so that you'll get a rich text editor box instead of a textbox, or you can change the default text box into a check box by setting the type to "Boolean". 
<br />
<br />
{
"Id": "TwitterId",
"Title": { "key": "", "default": "Twitter ID" },
"Help": { "key": "", "default": "" },
"Type": "Boolean",
"Groups": [{ "key": "", "default": "Social" }],
"DefaultValue": { "key": "", "default": "" },
"Settings": {
}
<br />
<br />
The conclusion is that SharpLook defies the rigid rules of DNN by providing you with this ability to create/add different page settings if you want some of them to be per portal or per host. 
<br />
<br />
These settings can be used in templates Header default - you can access the custom header settings in the main.xsl file from:

\Portals\_default\Skins\SharpLook\templates\headers\default, for example:
  <xsl:value-of select="/SharpLookConfig/Settings/FacebookId/Value"/>. 