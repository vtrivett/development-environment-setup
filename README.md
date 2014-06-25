#Setting up a good development environment on a Mac

## Please feel free to correct or add suggestions.

###Xcode:
* Download Xcode from the App store. It will take a while so do this first.
* Install all updates for your OS etc.

###Sublime Text 3:
* [Download](http://www.sublimetext.com/)
* [Package control](https://sublime.wbond.net/installation)
* Emmet
* Sublime Linter
* Set up [subl command line shortcut](http://stackoverflow.com/questions/16199581/opening-sublime-text-on-command-line-as-subl-on-mac-os)
* Some settings to get you started:

````
{
	"bold_folder_labels": true,
	"color_scheme": "Packages/Color Scheme - Default/Solarized (Light).tmTheme",
	"fade_fold_buttons": false,
	"highlight_line": true,
	"highlight_modified_tabs": true,
	"ignored_packages":
	[
		"Vintage"
	],
	"line_padding_bottom": 1,
	"line_padding_top": 1,
	"word_wrap": true,
	"font_face": "AnonymousPro",
	"font_size": 18
}
````
###iTerm2:
* [Download](http://www.iterm2.com/#/section/home)
* I highly recommend a [heads-up terminal](http://ivanvillareal.com/osx/setup-iterm2-to-behave-like-guake/) for running servers and a good color scheme such as [solarized](https://github.com/altercation/solarized/tree/master/iterm2-colors-solarized).

###Other Apps:
* Alfred
* Dash
* Spectacle
* Skype
* Dropbox

###System preferences:
* *Dock*: Shrink the dock. 
* *Mission Control*: Set up hot corners for mission control and show desktop.
* *Displays*: Arrangement-> uncheck mirror displays, arrange second monitor to your liking. 
* *Trackpad*: Tap to click, X scroll direction, X swipe between pages 

###Chrome:
* Set up gmail, drive, and 2-factor authentication
* Suggested Extensions:
**JSONView

###Homebrew
````
ruby -e "$(curl -fsSL https://raw.github.com/Homebrew/homebrew/go/install)"
````

* Homebrew will ask you to download Xcode command line tools. When finished, run: 

````
brew doctor
brew update
````


###Git and Github
* Git config:

````
git config --global user.name "First Last"
git config --global user.email "flast@2u.com"
````


###Generate SSH keys:
* Instructions:

````
cd ~/.ssh
ssh-keygen -t rsa -C "you@2u.com"
#don't enter a passphrase
pbcopy < ~/.ssh/id_rsa.pub
````
* Paste the resulting RSA key to [Github](https://github.com/settings/ssh) and send to Helpdesk.

###Python, pip and virtualenv

`````
brew install python # python come with OSX but this installs pip and some other stuff
pip install virtualenv
`````

###Mongodb
* Installation with homebrew:

````	
brew install mongodb
````
* To start mongodb server, run ```` mongod ```` 
* For a shell, just type ```` mongo ```` 





