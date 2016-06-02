# Uninstalling Sharp Look

As you already know, Sharp Look is a skin and it can safely uninstalled just like any other skin or module. The only condition before proceeding with the uninstall process is to remove Sharp Look from the pages where is set as skin or delete those pages entirily. As you can see in the screenshot below, you can't uninstall it if it's on at least one page, because the bin pictogram is not visible:


![](2016-06-02_1616.png)

After you remove Sharp Look from all pages the bin pictogram becomes visible and it can safely uninstalled:


![](2016-06-02_1618.png)

You can find the Sharp Look skin under the Host - Extensions, and then click on the "Themes" in order to open the drop-down with the list of skins.

If you're not sure on what pages do you use the Sharp Look skin or the "bin" button does not show up, go to Host - SQL and run the following Query:

```select * 
  from tabs
  where SkinSrc like '%sharp%'
  or ContainerSrc like '%sharp%'```
  
  This will search the database for the keyword "sharp" and it will display a list with pages and portals where Sharp Look is being used.