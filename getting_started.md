# Getting Started

How to use Sharp Look

To sum up, Sharp Look is a CMS framework which redefines how sites are created and managed by replacing the DNN administration controls with a touch-friendly interface and which gives you the possibility to edit the design of your web pages, besides other options like View, Edit, Layout. 

Sharp Look let's you control your portal’s styling, it changes the entire DNN interface, it integrates as a skin, you can set is for a page or for the entire site, so basically, we say that Sharp Look is an engine. The purpose of Sharp Look is to get rid of as much UI as possible - we've build a DNN light distribution using this SharpLook engine on top of DNN, so basically we've refactored DNN a little to be able to get rid of all the UI. 
How to work with Sharp Look


There are two basic ways to integrate Sharp Look on your site, you can set your site with Sharp Look skin from Admin > Site Settings or from Host > Site Settings or you can use Sharp Look as skin per page. 
How to create a customized page with Sharp Look

First begin with the same steps you follow when you want to create a page: access Pages option from menu and click on Add new page, fill in all the fields which you consider you need and, the most important step in achieving our goal of creating a skinned page in Sharp Look, access Advanced Settings option and set Host: SharpLook option on both Appearance options - on Page Skin and on Page Container and finally, click on Add page button. Instead of a white canvas, all the existing page templates will be displayed and you'll have to choose one of them which you want to be used - you can select the Blank option if you need to get started from a white canvas, or some other templates which come with the Sharp Look package installation, you'll recognize them after their name which contains "SharpLook" in the title:

![](choose.template.png)

Once the template is selected, you'll get redirected in just fractions of a second to the created page which will be displayed according to the selected template and the Admin Control bar will be available and will provide the necessary options to go further in customizing the page - the options available are as follows:

the cogwheel icon button which enables the Control Panel page where there are displayed the available features per page/per portal/per host and an advanced Feature Search box which is useful to navigate between options, along with Clear Cache and Recycle application domain buttons.

![](control.panel.png)

View mode button which is destined for the end-users, in View mode, the page displays the final page after it was designed and edited according to the specifications.

Edit mode which is created for content editors who'll deal with the integration of the module per page and their customization (here all the module's settings options get displayed when you click on the + icon: Manage module, Settings of the module, Export/Import options, Help, Refresh and also Remove).

Layout mode which gives the ability to create rows and panes where the modules will be added into, you can also add modules here, so you're not strictly dependent on Edit mode to do this, and from Layout mode you can also control the Menu and the Header options. 

Design mode offers the possibility to customize the whole page by accessing the Edit page button - here, besides playing with colors, video, images, border sizes, you can also set Less styles in a certain format (e.g. background-color: red;) and you can also directly upload .css and/or .js files. There are also the Edit Row options which will let you customized each row if you need an interactive design. 

Pin button - the last option in line, has the purpose of rearranging the Admin Control bar to the right side of the page - the buttons will change to icons and whenever in doubt you can mouse over them to see what you have to click in order to access the mode you need. 

Exercise:

1. Create a page and set it to Sharp Look skin > chose the Blank template;

2. Access Layout mode and split the default row into two panes - increase the size of the Content Pane to the right by clicking on the arrow displayed in the right corner;

3. While you're still in Layout mode, check the Display Header box and the Enable Menu and Enable Registration Controls options > save;

4. Go to Edit mode and on first pane, the left one add an HTML module - add content in it and on the right pane, the second one add an ActionForm module with, let's say three text boxes and one submit button;

5. Now access Design mode and let's set a background image on row 1 and a color on header > save the modifications and see the final result by accessing the View mode.

6. Let's also put a phone number on the page by opening Control Panel page (click on the cogwheel icon button - the first button from the Admin Control buttons) > click on Page Settings icon > click on Social in order to enlarge the social options list > set a phone number in the last textbox > and click on Update page button

7. If you decide to use the customized page as a template or theme you can use the Create Theme button which will be displayed at any modification you'll make on Layout, Edit and Design page or the Export page button from Control Panel. The themes and templates are useful if you want to use the design and content between the pages of a website. 