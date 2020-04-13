# SVELauncher

## Installation and Use Instructions

### Download and Install Stardew Valley Expanded Launcher.app

1. Download the latest version from the Releases section in this repository.
2. Find the Stardew Valley Expanded.app.zip file that was just downloaded and decompress it by double-clicking it.
3. Move the resulting Stardew Valley Expanded Launcher.app to the Applications folder, or to a location of your choosing.

### Install the Mods

*The mods need to be installed in a specific folder so the application can load them.*

#### The easy way

1. Create a folder named Mods-SVE in the same folder where the default Mods folder is located.
(If you use Steam the location is /Users/YOURUSERNAME/Library/Application Support/Steam/steamapps/common/Stardew Valley/Contents/MacOS/)
2. Install the mods required for Stardew Valley Expanded and any of your other favorite mods in the Mods-SVE folder.

#### The Less Easy, but Better Way

You probably have a bunch of other mods already installed in the default Mods folder, which you would also would like to use with Stardew Valley Expanded, but you don't want to install them a second time, because who in their right mind would want to manage the same mods twice? Not me!

1. Open Terminal.app (don't be afraid)
2. Enter the following command and tap the return key
`mkdir ~/Library/Application\ Support/Steam/steamapps/common/Stardew\ Valley/Contents/MacOS/Mods-SVE`
3. Now enter the following command and tap the return key
`ln -s ~/Library/Application\ Support/Steam/steamapps/common/Stardew\ Valley/Contents/MacOS/Mods/* ~/Library/Application\ Support/Steam/steamapps/common/Stardew\ Valley/Contents/MacOS/Mods-SVE/`
4. Install the mods required for Stardew Valley Expanded in the Mods-SVE folder.

Are you wondering what the heck just happened? Well, in the first step you decided you were going to use Terminal.app. If you stepped outside your comfort zone, congratulations! It wasn't that bad, was it? In the second step you made a new folder named Mods-SVE in the proper location. Here's where it gets cool. In the third step you made super-duper alias, really called a symbolic link, of all the mods installed in your default Mods folder inside the Mods-SVE folder you made in step two. Why did you do this? I'm glad you asked. They're not really folders. Like I said previously, they're just super-duper alias that point back to their original folders in your default Mods folder. Any changes you make will affect both installations. For example if you edit the config.json file it will affect both sets of mods. If you update a mod it will affect both sets of mods. The only catch is if you delete the original folder, the super-duper alias will lose its connection. When updating mods always edit or replace the contents of the folder. Finally, in the fourth step you installed the mods required for Stardew Valley Expanded in addition to all your other favorite mods that were already "installed" in step three.

### Opening Stardew Valley Launcher.app

*If you double click to open the app you will receive a dialog box stating "Stardew Valley Expanded Launcher.app" cannot be opened because the developer cannot be verified. This is becasue the app is not signed with a certificate issued by Apple. See: https://support.apple.com/guide/mac-help/open-a-mac-app-from-an-unidentified-developer-mh40616/mac*

1. Right-click on the Stardew Valley Launcher.app and choose Open from the contextual menu.
2. Click the Open button in the dialog box.

### Uninstalling Incompatible or Unwanted Mod Installed Using The Less Easy, but Better Way

*The will not affect the installation in the original Mods folder.*

1. Throw the super-duper alias from the Mods-SVE folder in to the Trash to "uninstall" it.

### Installing Additional Mods for Stardew Valley Expanded

1. Install the mod using the standard procedure in the Mods-SVE folder.

### Installing Additional Mods for default and Stardew Valley Expanded

#### The Easy Way

1. Install the mod using the standard procedure in the default Mods folder.
2. Install the mod using the standard procedure in the default Mods-SVE folder.

#### The Less Easy, but Better Way

*In the example below we're going to install Content Patcher. In the command below replace ContentPatcher with the name of folder of the mod you want to install*

1. Install the mod using the standard procedure in the default Mods folder.
2. Open Terminal.app (You're an ol' hack by now).
3. Enter the following command and tap the return key
`ln -s ~/Library/Application\ Support/Steam/steamapps/common/Stardew\ Valley/Contents/MacOS/Mods/ContentPatcher ~/Library/Application\ Support/Steam/steamapps/common/Stardew\ Valley/Contents/MacOS/Mods-SVE/`
