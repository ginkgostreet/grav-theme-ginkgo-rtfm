# Ginkgo RTFM

The Ginkgo RTFM theme is a customized version of the default [Grav Learn](http://learn.getgrav.org) theme, and includes some extra configurable options:

- Logo URL

# Installation

Installing the Ginkgo RTFM theme can be done in one of two ways. Our GPM (Grav Package Manager) installation method enables you to quickly and easily install the theme with a simple terminal command, while the manual method enables you to do so via a zip file.

The theme is designed to be used to provide a documentation site. You can see this in action at [learn.hibbittsdesign.org](http://learn.hibbittsdesign.org)

## GitHub Installation (Preferred)

The simplest way to install this plugin is via Git on the command line.  In the `/user/themes` directory your Grav install type:

```shell
$ git clone https://github.com/ginkgostreet/grav-theme-ginkgo-rtfm ginkgo-rtfm
```

This will  the Ginkgo RTFM theme into your `/user/themes` directory within Grav. Its files can be found under `/your/site/grav/user/themes/ginkgo-rtfm`. 

## Manual Installation

To install this theme, just download the zip version of this repository and unzip it under `/your/site/grav/user/themes`. Then, rename the folder to `ginkgo-rtfm`. You can find these files on [GitHub](https://github.com/ginkgostreet/grav-theme-ginkgo-rtfm).

You should now have all the theme files under

    /your/site/grav/user/themes/ginkgo-rtfm

>> NOTE: This theme is a modular component for Grav which requires the [Grav](http://github.com/getgrav/grav), [Error](https://github.com/getgrav/grav-theme-error) and [Problems](https://github.com/getgrav/grav-plugin-problems) plugins.

### Recompile CSS from SCSS

To recompile default style using a Sass-compiler, run it on /scss/theme.scss and output to /css/theme.css, like `node-sass --watch --source-map true scss/theme.scss css-compiled/theme.css`. To do the same for custom styles, run it on /scss/custom and output to /css-compiled/custom, like `node-sass --watch --source-map true scss/custom/ css-compiled/custom`.

## Features

* Lightweight and minimal for optimal performance
* Fully responsive with off-page mobile navigation
* SCSS based CSS source files for easy customization
* Built specifically for providing easy to read documentation
* Fontawesome icon support

### Supported Page Templates

* "Docs" template
* "Chapter" template
* Error view template

## Setup

If you want to set Ginkgo RTFM as the default theme, you can do so by following these steps:

* Navigate to `/your/site/grav/user/config`.
* Open the **system.yaml** file.
* Change the `theme:` setting to `theme: ginkgo-rtfm`.
* Save your changes.
* Clear the Grav cache. The simplest way to do this is by going to the root Grav directory in Terminal and typing `bin/grav clear-cache`.

Once this is done, you should be able to see the new theme on the frontend. Keep in mind any customizations made to the previous theme will not be reflected as all of the theme and templating information is now being pulled from the **ginkgo-rtfm** folder.

## To Do

- Make page numbers in nav a configurable option in the theme
- Make hiding sub-menu and sub-sub-menu items if parent(s) not active a configurable option in the theme
- Create theme option for configuring which page templates will display the TOC plugin