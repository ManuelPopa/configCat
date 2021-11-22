# configCat
config cat

Config Cat is a sample login page for the sole purpose of testing an easy implementation of ConfigCat's feature toggle funtionality

For this test I used the CDN integration version : <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/configcat-js@latest/dist/configcat.min.js"></script>
An account is needed in order to get a SDK Key - it can be created here https://app.configcat.com/signup
Once the account is active you'll have to go to the top right corner where there's a button "SDK Key". Click it in order to copy the key.

A default feature key is present once the account is created, and it has a switch in order to activate/deactivate it.

In the sample page, I then created the client using my key and then called the .getValue function in order to get the value of the feature toggle when the page is loaded.
This value is stored in a variable, "isMyFirstFeatureEnabled", which I then use to redirect the authenticated user to google (if the toggle is off) or duckduckgo (if the toggle is on).

The entire process of setting up the account and using a feature toggle from ConfigCat is less than 10minutes long. Thanks in part to their great documentation: https://configcat.com/docs/getting-started/

 