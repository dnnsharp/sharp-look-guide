# FAQ

**How to customize the header**
<br />
<br />
If you need to customize the menu in Sharp Look without affecting other portals you can do it on the page in Design mode > click on Edit Header > expand the More Styles box and type your CSS there. For example, if you need to modify the position of the menu options and shift it more to the left, you can type:
<br />
<br />
.navbar-collapse{position:relative;left:-100px;}.
<br />
<br />
**How to set up a link which, when clicked, will scroll down to the next row**
<br />
<br />
To do this, just create a link to the same page and append the the ID of the row as URL fragment. For example, ```/mypage.aspx#dnn_slkRow24```.
<br />
<br />
**How to customize the Login and Registration pages**
<br />
<br />
In a JS file add the following code:
<br />
<br />
$(function(){

_.each($('.slk-login-register'), function(x){$(x).find('a:first').attr('href', '/login_link')});

_.each($('.slk-login-register'), function(x){$(x).find('a:nth-child(2)').attr('href', '/register_link')});

});
<br />
<br />
and upload it in Design Mode. Replace /login_link and /register_link with your desired links.
