# Just Not Sorry -- the Gmail Plug-in
Inspired by the writings of Tara Mohr and others, this Chrome Extension for Gmail will warn you when you use phrases that might be undermining your message.

## Citations
  * http://www.taramohr.com/8-ways-women-undermine-themselves-with-their-words/
  * http://goop.com/how-women-undermine-themselves-with-words/
  * http://www.fastcompany.com/3032112/strong-female-lead/sorry-not-sorry-why-women-need-to-stop-apologizing-for-everything
  * http://www.fastcompany.com/3049609/the-future-of-work/4-types-of-useless-phrases-you-need-to-eliminate-from-your-emails
  * http://jezebel.com/google-exec-women-stop-saying-just-so-much-you-sound-1715228159
  * http://www.lifehack.org/articles/communication/7-things-not-to-say-and-7-things-to-start-saying.html

## Contributing

### Requests to add or change warning phrases
Please [create a GitHub issue](https://github.com/cyrusinnovation/just-not-sorry/issues/new) with your request.  If you're a developer, you're welcome to submit a pull request.

### Development Setup
  * `git clone` the repo
  * Follow the [instructions on the Chrome docs](https://developer.chrome.com/extensions/getstarted#unpacked) to load the extension
  * Go to Gmail and open a compose window
  * If you make changes to the code, click the Reload link on the `chrome://extensions` page and then reload your Gmail tab to pick up the changes.
  * Errors will show up in the console

### Coding Standards
Use [JSCS](http://jscs.info/) with the AirBnB preset.

### Jasmine Tests
Open 'SpecRunner.html' in your web browser to run the test suite.
    
### To Publish to Chrome Webstore
  * Update the version number in `manifest.json`
  * Run the `package.sh` shell script to generate a zip file
  * Go to [Chrome Developer Dashboard](https://chrome.google.com/webstore/developer/dashboard) and edit the existing app. Upload the new zip file and then publish the changes (button is at the very bottom).

### Libraries Used
For production:
  * [gmail.js](https://github.com/KartikTalwar/gmail.js)
  * [findAndReplaceDOMText](https://github.com/padolsey/findAndReplaceDOMText)
  * [jQuery](https://jquery.com/)
  * Based on [gmail-chrome-extension-boilerplate](https://github.com/KartikTalwar/gmail-chrome-extension-boilerplate)

For test:
  * [jasmine.js](http://jasmine.github.io/)
  * [jasmine-jquery.js](https://github.com/velesin/jasmine-jquery)
