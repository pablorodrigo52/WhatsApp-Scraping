# :speech_balloon: WhatsApp-Scraping
Python script to get WhatsApp information from WhatsApp Web

# Requirements 
All the libraries that we are going to use are in the [requirements.txt](requirements.txt) file.
You can install it with PIP in the terminal with:
```
sudo pip install -r requirements.txt
```
In order to make this project work you need to have a profile in your browser where you already scanned the QR with your account then we are going to use that account for launching the Selenium driver.

## Selenium
Selenium requires a driver to interface with the chosen browser. Firefox, for example, requires geckodriver, which needs to be installed before the below examples can be run. Make sure it’s in your PATH, e. g., place it in /usr/bin or /usr/local/bin.

Failure to observe this step will give you an error selenium.common.exceptions.WebDriverException: Message: ‘geckodriver’ executable needs to be in PATH.

Other supported browsers will have their own drivers available. Links to some of the more popular browser drivers follow.
* [Chrome](https://sites.google.com/a/chromium.org/chromedriver/downloads)
* [Edge](https://developer.microsoft.com/en-us/microsoft-edge/tools/webdriver/)
* [Firefox](https://github.com/mozilla/geckodriver/releases)
* [Safari](https://webkit.org/blog/6900/webdriver-support-in-safari-10/)

# Settings
**AT THIS MOMENT WE HAVE THE CODE ONLY WORKING FOR FIREFOX**

## Browser Profile ```FIREFOX_PATH```
You need to setup your configuration in the [settings.txt](settings.txt) file.
In this file you need to specify the profile of your browser where you already scan the QR whit your WhatsaApp account

For example we are using the default Firefox profile so we open Firefox and go to https://web.whatsapp.com/ then we scan our QR to login then we can close Firefox and go to search for our profile file that we have in ```/home/user/.mozilla/firefox/xxxxxxxx.default```, now that we localized our file we add the direction to our [settings.txt](settings.txt) file in the FIREFOX_PATH

