![iDownloader App Icon|100x100](iDownloader-iOS-Default-1024x1024@2x.png)

**iDownloader**


iDownloader is the easiest way to distribute your apps using the power of AppleScript.

---

**Why it works, and why you should use it too**


iDownloader is so simple you can easily distribute ALL your apps in just 5 minutes! With iDownloader, all you have to provide is a array of your Apps and the locations to their DMGs on your server. Take mine for example:


```
set appsList to {¬
	{name:"Rocket", downloadURL:"https://jbluebird.github.io/Install-My-Apps/Install%20Rocket.dmg", internalName:"Rocket"}, ¬
	{name:"iCompress", downloadURL:"https://jbluebird.github.io/Install-My-Apps/Install%20iCompress%20Beta%201.1.dmg", internalName:"iCompress"}}
```
This is my array that I use for distributing all my apps with iDownloader. I will explain this and how it works. Take my app Rocket for example:

```
{name:"Rocket", downloadURL:"https://jbluebird.github.io/Install-My-Apps/Install%20Rocket.dmg", internalName:"Rocket"}
```

```name:"Rocket"``` is the display name in which the app will appear in the install app picker.
```downloadURL:"https://jbluebird.github.io/Install-My-Apps/Install%20Rocket.dmg"``` is the location of the app DMG on your server.
Finally, ```internalName:"Rocket"``` is the .app file's name inside your DMG. In my case, in my Install Rocket DMG, the .app file inside is named Rocket.app, so I will put in ```Rocket```
