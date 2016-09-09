## Synopsis

McBoots Child is a starter child theme for the [McBoots](https://github.com/donnamcmaster/mcboots) WordPress template. It is deliberately minimal. 

Note that both McBoots and McBoots Child assume that you are familiar with both WordPress and PHP programming. They are not intended for novices. 

## Motivation

Although we could simply edit McBoots directly, creating child themes enables us to more easily update the core code without impacting all sites based on McBoots. 

## Organization

McBoots Child consists of the following:

* License and read-me files that can be modified or ignored. 
* An `assets` folder with sub-folders for CSS, fonts, images used in styles (e.g., logo, icons), Javascript, and LESS files. 
* Empty folders `lib`, `lib/setup`, and `template-parts`. When you need to override a file in the McBoots parent theme, copy that file into the matching folder in McBoots Child and edit it as needed. 
* WordPress standard file `style.css`. NOTE: This file is only to satisfy WordPress theme requirements. The actual site CSS is generated from LESS files and is located in `assets/css`.
* Theme image file `screenshot.png`. Replace if desired. Recommended size is 1200 x 900 px. PNG or JPEG files work well. 

## Installation

* First download McBoots and install it in a `mcboots` (lower case) folder in your `wp-content/themes` folder. 
* Then download McBoots Child and install it in a folder in your `wp-content/themes` folder. We suggest that you change the folder name and edit `style.css` to change the theme name and details at this time. 
* Select your copy of McBoots Child in WordPress admin (Appearance/Themes). 

## Setup

I'm not including build files with the project at this time. The only file that needs compilation is `assets/less/app.less`. It is compiled into `assets/css/app.css`. `App.less` includes the bootstrap files. 

I made one modification, to pick up `variables.less` from a copy in assets/less instead of from assets/less/bootstrap. This is because I find it easier to set colors, fonts, and other values in `variables.less` rather than overriding them later. If you prefer not to touch the Bootstrap distro, edit `assets/less/bootstrap/bootstrap.less` to pick up `variables.php` from the bootstrap directory instead. 

See also the [McBoots documentation](https://github.com/donnamcmaster/mcboots). 

## Contributors

I appreciate your letting me know (via message or pull request) if you find any problems or see areas for improvement. You can contact me [via email](https://www.donnamcmaster.com/contact/ "at my website") or on Twitter as [@mcdonna](https://twitter.com/mcdonna). 

## License

Licensed under [GPLv3 or later](https://www.gnu.org/licenses/gpl.html).
