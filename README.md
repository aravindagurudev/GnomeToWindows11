# Conversion of Gnome Linux environment to Win 11 

Hi! below are the steps to Convert your **Gnome** desktop environment to **Windows 11** theme. Here you will learn customise **Gnome**, adding **themes**, working with **extensions**, customising extensions e.t.c.

# Steps are as follows:
## 1. Install Git to you Linux desktop.
- **Debian :** apt install git
- **RHEL :** dnf install git
- **Arch :** sudo pacman -S git
- **Nix OS :** nix-env -i git
- **Open SUSE :** zypper install git
## 2. Install gnome-tweaks and gnome-extension-manager
- **gnome-tweaks**
	- Install gnome-tweaks via software installer or command line of your Linux.
- **gnome-extension-manager**
	- Generally this will be available via third party software installers so use software centre to search and install.
	- After installing check if ***user-themes*** extension is available if available enable it.
 > if user-themes not available then install it by **browsing the extensions** and after installing enable it.
## 3. Install Themes
- **Windows 11 Icon Theme:** 
	- Git Repository to download : git clone https://github.com/yeyushengfan258/Win11-icon-theme
	- Navigate to Win11-icon_theme folder and run `sh install.sh` to install the theme.
- **Windows 11  Appearance (Look and Feel) theme :** 
	- Git Repository to download: 	git clone  https://github.com/vinceliuice/Fluent-gtk-theme
	-  Navigate to Fluent-gtk-theme folder and run `sh install.sh` to install the theme.
## 4. Enable Themes
- Open **gnome-tweaks** Click on **Appearance** menu left side.
- Go to **Icons** select **Win11** under the drop-down menu.
- Go to **Shell** select **Fluent-Dark/Fluent-Light** for dark or light mode from drop-down.
- Go to **Applications/Legacy Applications** and select **Fluent-Dark/Fluent-Light** from drop-down.
> **Your theme and Icons are set now!!!**
## 5. Install Font
- Font used by Windows is `segoe-ui` search in the google and install it on your Linux environment.
	- example: https://freefontsfamily.com/segoe-ui-font-free/#google_vignette
- Open **gnome-tweaks** select fonts menu from left side change interface text font to `segoe-ui` (regular/light).

## 6. Extensions
Open Extensions Manager select browse menu on the top and Install following extensions and change settings as given.
- **1. Dash to panel**
	-  Install extension ***Dash to Panel*** extension by `charlesg99`.
	- **Settings**:
		-  Under **Position** tab do following:
			- Disable `'Show Applications Button'` (Click on Visible button so that highlight is removed).
			- For the `'Left Box'` set drop-down to `Monitor Center`
			- For the `'Taskbar'` set drop-down to `Monitor Center`
		- Under **Style** tab do following:
			- Change `'App Icon Margin'` to zero.
			- Change `'App Icon Padding'` to 6.
			- Under `'Running Indicator'` change running indicator style focused and unfocused to `Dashes`
		- Under **Behaviour** tab do following:
			- Search for `Disable show overview on startup` and enable the option.
		- Under **Fine-Tune** tab do following:
			- Change all font size to **16**.
			- Change all padding to **4 pixel**
- **2. Arcmenu** 
	- Install  ***Arcmenu***  extension by `andrew.zaech`.
	- **Setting up**: Click on `Arcmenu` gear(settings) icon on installed extensions tab.
		- Under **General** tab:
			- Enable `Display Arcmenu on all Panels`.
		- Under **Menu** tab:
			- Select `Menu Layout` under that select `Modern Menu Layouts` under that select `11` and return.
			- Select `Menu Visual Appearance` and do following change:
				- Change `Height` to  750.
				- Change `Left-Panel Width` to 175.
				- Under `Override Icon Sizes`change `Application` drop-down to `Large`.
			- Select `Fine Tune` Disable `Alphabetize 'All Programs' Category`.
		- Under **Menu Button** tab:
			- Change `Padding` under `Menu button appearance` to 5.
			- Change `Icon Size` under `Menu Button Icon` to 33.
			- Browse `Choose new Icon` under `Menu Button Icon` select custom and use the image `'WindowsMenu.png'` under `'assets'` folder of this repository.
- **3. Blur my Shell**
	- Install ***Blur my Shell*** extension by `aunetx`
	- **Setting Up :** Click on `Blur my Shell` gear(settings) icon on installed extensions tab.
		- Click on Panel tab down and do following:
			- Enable `'Customize properties'` under that set `Sigma` to `15` and `Brightness` to `1`. 
- **4. Date Menu Formatter**
	- Install *** Date Menu Formatter*** extension by `mjakubowski`.
	- **Setting Up :** Click on `Blur my Shell` gear(settings) icon on installed extensions tab.
		- Change `Pattern` to `dd/MM/yy\nhh : mm aa`
- **5. Media Controls**
	- Install *** Media Controls*** extension by `cliffniff`.
	-  **Setting Up :** Click on `Media Controls` gear(settings) icon on installed extensions tab.
		- Under `Visibility` tab do following:
			- Enable `Colored player icon`.
			- Turn off `Title/Track name`, `Player controles` and `Sources Menu`.
		- Under `Position` tab, change extension position to `right`
		- Under `Other` tab, change left click to `Open track information menu` and make all other to `None`

## 7. DMZ white cursor theme.
- Open **Gnome tweaks** and click on **Appearance** and try to  change cursor theme to **Dmz-white**
- **Dmz-White** not available then do following:
	- Download the them zip file from https://www.gnome-look.org/p/999299
	- Extract the downloaded zip file you will get folder `DMZ-White`.
	- Copy the folder to .icons folder in user root (If .icons folder not present create it).
	- Open gnome-tweaks (close and open if already opened).
	- Under **`Appearance`** menu select **`'Cursor themes'`** to **`DMZ-White`**
## 8. Desktop Wall Papers
-  I have provided wall papers in assets folder both Dark and Light they can be used or any other wallpaper can be used.

> **Done Customising the gnome environment and you will be in Windows 11 theme**
# Done


## Known bugs and fixes:
> - **Extension Manager not found :**
	- Try to install Extension manager from third party enabled or from flat-hub or from snap package manger.
> - **Arcmenu Disabled**
	> 	- Try to check what is the error and install missing packages and install them, OR other way is directly install extensions by searching with package manage for example in case of nix os: `nix-env -i gnome-shell-extension-arcmenu` run this command to install extension.
> - **Extension are not showing up in browse tab of Extension Manager :**
	- Some times Gnome extensions website will be down because of this you will ot find any extensions in such situations wait for some time and try again.


