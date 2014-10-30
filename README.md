# SocialShare

SocialShare is a CommonJS Module for Titanium that implements cross-platform sharing of text and images over social networks.

## iOS
On iOS, the module uses the native sharing Action Sheet and offers options for sharing with Facebook and Twitter (if the native apps are installed), 
plus AirDrop, Text Message, Email and other built-in iOS mechanisms.

## Android
On Android it uses the Native Sharing Intent, which brings up a list of installed apps to choose from.

![](http://drops.ricardoalcocer.com/drops/ios_android_sharing-y54AvtkxtS.png)

## Usage

If you want to send an email, set the image property to the Native Path to the image.  If you wish to only send text, simply don't send the image property.
```javascript
require('com.alcoapps.socialshare').share({
	status 					: 'This is the status to share',
	image 					: fileToShare.nativePath,
	androidDialogTitle 		: 'Sharing is caring!!!'
})
```

**BOOM!  That's it!  You're sharing!**

## Dependencies	
This module requires dl.napp.social for iOS which you can get from [https://github.com/viezel/TiSocial.Framework](https://github.com/viezel/TiSocial.Framework)

## Get it
You can get it from the [/app/lib](https://github.com/ricardoalcocer/socialshare/tree/master/app/lib) folder.

## Credits
This module borrows from from code and ideas by:

* [Mads Møller](https://github.com/viezel/)
* [Adam Paxton](https://github.com/adampax/)
* [Dan Tamas](https://github.com/rborn)

## License
[MIT - http://alco.mit-license.org](http://alco.mit-license.org)