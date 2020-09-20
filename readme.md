<!-- @format -->

# (HR) Grande Omega Skins

This is a collection of unofficial skins for Grande Omega. It changes and adds some files to make Grande Omega appear in your preferred skin.

**Use at your own risk, We're not responsible for any errors, bugs, or other stuff you might run into.**

### You're not allowed to use any of the skins during exams / tests, make sure you have a clean copy!

## Skins

### Fox Dark - Foxxite

![](skins/fox-dark/screenshots/1.png)
![](skins/fox-dark/screenshots/2.png)
![](skins/fox-dark/screenshots/3.png)

### Wumpus Dark - VAC Efron

![](skins/wumpus-dark/screenshots/1.gif)
![](skins/wumpus-dark/screenshots/2.png)
![](skins/wumpus-dark/screenshots/3.png)

## Installation

Download the repo using the "**↓** Code" button and select the ZIP file.

Make a **copy** of the resource folder in the Grande Omega folder.

### Resource folder locations

**Normal Version**: `Grande_Omega\resources`

**Auto Updater Version**: `Grande_Omega\tmp`

---

Place the `themes` folder inside of

**Normal Version**: `Grande_Omega\resources\app\desktop\Student\wwwroot`

**Auto Updater Version**: `Grande_Omega\tmp\wwwroot`

for the code editor themes to work.

## Skin Installation

In the zip file go to the folder **skins** and pick a skin you want to use.

### Steps Normal Version

Extract the contents of your chosen skin folder from the zip file **on top** of your Grande Omega directory.

### Steps Auto Updater

Go into the folder of you chosen skin until you find the files and folders `index.html, main.js (not always included) and wwwroot`.
Extract these files **on top** of `Grande_Omega\tmp\`.

---

Replace the files you get asked to replace.
Next time you start grande Omega it should appear in your chosen skin.

To change skin, restore the recourse folder from the copy you made and repeat the installation steps.

## Contributing

Fork this repo and clone it to your workspace.

Create your own skin by making a folder for your skin in the skins folder.
We recommend to use Fox Dark as a starting point.

Make sure to add screenshots of your theme to this ReadMe file.
And to update the skin.json file with he correct information.

Create a pull request on this repo with a branch sharing the name of your theme.
Once your theme has been approved it will be merged into the master branch.

If you haven't already setup signed commits, these look nicer :)

Any skins that **edit any non CSS (except index.html and main.js)** files will be declined.

### Skin.JSON structure

Make sure to remove the arrow comments or the JSON will not work

```JSON
{
	"name": "", <-- skin name
    "author": "", <-- skin author
    "version": 1, <-- skin version

	"resourceDir": "resources/app/desktop/Student", <-- location of modified files, should always be this
	"screenshotsDir": "screenshots", <-- location of screenshots

	"modifiedFiles": ["index.html", "wwwroot/css/style.css"], <-- modified files as seen from resourceDir
	"addedFiles": ["wwwroot/css/bootstrap-dark-min.css",], <-- added files as seen from resourceDir

	"screenShots": ["1.png", "2.png", "3.png"] <-- screenshot files as seen from screenshotsDir
}
```

### Dev Tools

To get access to the dev tools, replace the

**Normal Version**: `Grande_Omega\resources\app\desktop\Student\main.js`

**Auto Updater Version**: `Grande_Omega\tmp\main.js`

file with the one found in the root of the repo.
