# Awesome Xcode Scripts


[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/aashishtamsya/awesome-xcode-scripts)
[![Platform](https://img.shields.io/badge/platform-Xcode-lightgrey.svg)](https://developer.apple.com/xcode/)
[![Programming Language](https://img.shields.io/badge/language-shell-yellow.svg)](https://en.wikipedia.org/wiki/Shell_script)
[![license](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE.md)

A curated list of useful Xcode scripts 📝.

## Content
  
-	[How to Setup](#how-to-setup)
-	[Scripts](#scripts)
	-	[Build Number Auto-Increment Script](#build-number-auto-increment-script)
	-	[Build Number Auto-Increment Script on Git Commit](#build-number-auto-increment-script-on-git-commit)
	-	[Semantic Version Auto-Increment Script](#semantic-version-auto-increment-script)
	-	[AppIcon Versioning Auto-Increment Script](#appicon-versioning-auto-increment-script)
	-	[Detect FixMe ToDo Error Tag on Swift Script](#detect-fixme-todo-error-tag-on-swift-script)	
-	[Installation](#installation)
-	[Contributing](#contributing)
-	[Credits](#credits)
-	[License](#license)

## How to Setup

*	Open Xcode project. Select your target
*	Build Phases -> Add Build Phase -> Add Run Script Build Phase
*	Open "Run Script" section that was created and .
*	Copy & Paste your script there.
*	(Optional) Rename your Run Scripts to identify them easily.

![DEMO](/Resources/DEMO.gif)

## Scripts 

### Build Number Auto-Increment Script

*	[BuildVersion.sh](/Scripts/BuildVersion.sh)	-	A script that runs each time you build your app in Xcode to read the Build number, increment it, and write it back to the app's `{App}-Info.plist` file.

### Build Number Auto-Increment Script on Git Commit

* [BuildNumberOnGitCommit.sh](/Scripts/BuildNumberOnGitCommit.sh) - A script that runs each time you commit your app to git, the Build number gets incremented.

> **CAUTION**
>
> Use this only if you are pushing you code to git.

### Semantic Version Auto-Increment Script

* [VersionNumberIncrement.sh](/Scripts/VersionNumberIncrement.sh) - Auto-increment the version number (only) when a project is archived for export.

> **CAUTION**
>
> Insure your starting version number is in SemVer format (e.g. 1.0.0)


### AppIcon Versioning Auto-Increment Script

* [IconVersioning.sh](/Scripts/IconVersioning.sh) - Overlay the iOS application version on top of the icon.

### Detect FixMe ToDo Error Tag On Swift Script

* [DetectFixMeToDoSwift.sh](/Scripts/DetectFixMeToDoSwift.sh)

## Installation

1. Download the zip or clone the repo to your desired directory.

```sh
$ git clone https://github.com/aashishtamsya/awesome-xcode-scripts.git
```

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request 😉 😊
  
## Credits
  
*	[**Build Number Auto-Increment Script**](/Scripts//BuildVersion.sh) 
	- [Jason Horwitz](https://github.com/sekati)

*	[**Build Number Auto-Increment Script on Git Commit**](/Scripts//BuildNumberOnGitCommit.sh) 
	- [Jared Sinclair](http://jaredsinclair.com/)

*	[**Semantic Version Auto-Increment Script**](/Scripts//VersionNumberIncrement.sh)	
	- [Jason Horwitz](https://github.com/sekati)
	
*	[**AppIcon Versioning Auto-Increment Script**](/Scripts//IconVersioning.sh)	
	-	Inspired by [@merowing](http://www.merowing.info/2013/03/overlaying-application-version-on-top-of-your-icon/#.VCg9li5_v6A) and [@bejo](https://github.com/bejo/XcodeIconTagger/blob/master/tagIcons.sh) script, who were inspired initially by Evan Doll's talk
	
Aashish Tamsya [@ChiefAashish](https://www.twitter.com/chiefaashish),
aashish.tamsya@gmail.com 

## License

The content of [*Awesome Xcode Scripts*](https://github.com/aashishtamsya/awesome-xcode-scripts) itself is licensed under the [Creative Commons Attribution 3.0 license](https://creativecommons.org/licenses/by/3.0/us/deed.en_US), and the underlying source code used to format and display that content is licensed under the [MIT license](https://opensource.org/licenses/mit-license.php).

See the [LICENSE](LICENSE.md) file for more info.
