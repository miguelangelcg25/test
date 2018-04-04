<!DOCTYPE HTML PUBLIC>
<html lang="en">
    <head>
        <title>NoPasswordOpenAMAuth/README.md</title>
    </head>
    <body>
        <div>
            <img src="https://raw.githubusercontent.com/NoPasswordRepo/NoPasswordOpenAMAuth/master/images/nopassword_logo.png" width="198" height="44"/>
        </div>

        <h1><strong>NoPasswordOpenAMAuth</strong></h1>

        <p>The NoPassword OpenAM Authentication Module allows to ForgeRock users to integrate their AM instance to the NoPassword authentication services.</br>
            This document assusmes that you already have an AM 5.5+ instance running with an user base configured.</p>

        <h2><strong>Installation</strong></h2>

        <p>Follow this steps in order to install the module:</p>
        <ol>
            <li>Download the jar file from <a href="https://github.com/NoPasswordRepo/NoPasswordOpenAMAuth/blob/master/target/nopassword-openam-auth-module-1.0.jar">here</a>.</li>
            <li>Copy the **nopassword-openam-auth-module-1.0.jar** file on your server: /path/to/tomcat/webapps/openam/WEB-INF/lib</li>
            <li>Restart AM.</li>
            <li>Login into NoPassword admin portal and open the Keys menu on the left side. Copy the Generic API key value by clicking in the green button and save it for later.</li>
            </br><img src="https://raw.githubusercontent.com/NoPasswordRepo/NoPasswordOpenAMAuth/master/images/generic_api_key.png"></br></br>
            <li>Login into AM console as an administrator and go to Realms > Top Level Real > Authentication > Modules.</li>
            <li>Click on Add Module button. Name the module NoPassword and select NoPassword from Type list.</li>
            </br><img src="https://raw.githubusercontent.com/NoPasswordRepo/NoPasswordOpenAMAuth/master/images/add_module_1.png"></br></br>
            <li>Set the email domain from you organization.</li>
            <li>Set the Generic API Key. Paste you generic API key from step 4 here.</li>
            </br><img src="https://raw.githubusercontent.com/NoPasswordRepo/NoPasswordOpenAMAuth/master/images/add_module_2.png"></br></br>
            <li>Save changes.</li>
            <li>You can test the NoPassword authentication module by accesing this URL in your browser https://<strong>your_AM_server here</strong>/openam/XUI/?realm=/#login/&module=NoPassword.</br>
                Enter your username and hit enter. You should get an authentication request on your phone.</li>
            </br><img src="https://raw.githubusercontent.com/NoPasswordRepo/NoPasswordOpenAMAuth/master/images/demo_auth.png"></br></br>
        </ol>
    </body>
</html>
