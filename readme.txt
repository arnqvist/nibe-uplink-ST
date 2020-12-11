Note! This repository is no longer looked after. I dont know if this does work anymore.

Instructions:

Register free account at Nibeuplink.com and connect your pump with an ethernet cable, if your pump is fitted with one. Mine is, but its relative new and i dont know when they started mounting it. Then when you are at the overview page for your pump. Look in the adressbar and note down your System ID, it's right between "system" and "status".

Login to api.nibeuplink.com, go to "my applications" and create new. Call it what you want and set the callback url to "https://graph-eu01-euwest1.api.smartthings.com/oauth/callback". Then note down your "identifier" and "secret". And keep them secret.

Go to the SmartThings IDE and create SmartApp from the code nice-uplink-ST.groovy found at "https://github.com/arnqvist/nibe-uplink-ST/".

Go to that apps "app settings" and then under "settings" set clientId to your noted Identifier and clientSecret to your noted Secret from the API. Then enable Oauth, update and publish.

Go create a new Device handler from the code nibe-f750-tile.groovy found at the same repository as before. Since I'm new to this i don't know if you have to enable Oauth in the device handler or not. Publish.

Install the SmartApp and you will be asked to login to your Nibe UpLink account. Do that and when you see a white page (lol), click done and enter your noted System ID.
