<img src="iDownloader-iOS-Default-1024x1024@2x.png" alt="iDownloader App Icon" style="width: 200px;">

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

**With this info you put in, what can iDownloader do?**

iDownloader will:

- Download the DMG online into /var/tmp
- Mount the DMG
- Copy the app outside of the DMG onto the desktop (that's why specifying the .app name with ```internalName:``` in your DMG is so important)
- Make the app executable (if not already)
- Unmount the DMG and delete the DMG file downloaded

**Annd you are done!**

Just look at that beautiful installer you just created!

**iDownloader does that.**

It's all simple, with barely any info you need to put in to work.

**Licensing**

MIT, do what you want, but no promises that it might break 🙃
