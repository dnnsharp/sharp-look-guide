# Custom Page Settings

Summary
purpose is to provide custom specific settings to less than admins
open architecture, can be extend through config files and/or custom assemblies
settings can be of different types (Boolean, texts, etc.)
settings can be inherited from host scope to portal scope to page scope
settings can be locked for modification at any level
settings can be accessed from: 
Header template
HttpContext.Items (todo)
My Tokens (todo)
Building Block (todo)
This Settings engine lets the administrators to control the content of the website/page, it's an opened engine - in Config there's a .json file in PageVars which has all the existing settings defined, for example, TwitterId, FacebookId, LinkedInId and each one of them has some settings like Title, Type etc. If you want to change the type of the field, you can for example replace the default "text" type with the "textarea" type so that you'll get a rich text editor box instead of a textbox or, you can change the default text box into a check box by setting the type to "Boolean". 

{
"Id": "TwitterId",
"Title": { "key": "", "default": "Twitter ID" },
"Help": { "key": "", "default": "" },
"Type": "Boolean",
"Groups": [{ "key": "", "default": "Social" }],
"DefaultValue": { "key": "", "default": "" },
"Settings": {
}

To sum up regarding what you can do with this settings engine based on the examples provided above, is that SharpLook defies the rigid rules of DNN, by providing you with this ability to create/add different page settings if you want some of them to be per portal or per host. 

These settings can be used in templates Header default - you can access the custom header settings in the main.xsl file from:

\Portals\_default\Skins\SharpLook\templates\headers\default, for example:
  <xsl:value-of select="/SharpLookConfig/Settings/FacebookId/Value"/>. 