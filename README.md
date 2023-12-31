# Slickslider Plugin

The **Slickslider** Plugin is an extension for [Grav CMS](https://github.com/getgrav/grav). It creates a nice Image Slider on any Page of your Grav CMS Installation

## Demo
[https://hoernerfranzracing.de/werner/en/demo/slickslider](https://hoernerfranzracing.de/werner/en/demo/slickslider)

## Installation

Installing the Slickslider plugin can be done in one of three ways: The GPM (Grav Package Manager) installation method lets you quickly install the plugin with a simple terminal command, the manual method lets you do so via a zip file, and the admin method lets you do so via the Admin Plugin.

### GPM Installation (currently NOT available)

To install the plugin via the [GPM](https://learn.getgrav.org/cli-console/grav-cli-gpm), through your system's terminal (also called the command line), navigate to the root of your Grav-installation, and enter:

    bin/gpm install slickslider

This will install the Slickslider plugin into your `/user/plugins`-directory within Grav. Its files can be found under `/your/site/grav/user/plugins/slickslider`.

### Manual Installation

To install the plugin manually, download the zip-version of this repository and unzip it under `/your/site/grav/user/plugins`. Then rename the folder to `slickslider`. You can find these files on [GitHub](https://github.com/wernerjoss/grav-plugin-slickslider) or via [GetGrav.org](https://getgrav.org/downloads/plugins) currently NOT available.

You should now have all the plugin files under

    /your/site/grav/user/plugins/slickslider

> NOTE: This plugin is a modular component for Grav which may require other plugins to operate, please see its [blueprints.yaml-file on GitHub](https://github.com/wernerjoss/grav-plugin-slickslider/blob/main/blueprints.yaml).

### Admin Plugin

If you use the Admin Plugin, you can install the plugin directly by browsing the `Plugins`-menu and clicking on the `Add` button (currently NOT available, see GPM Installation above).

## Configuration

Before configuring this plugin, you should copy the `user/plugins/slickslider/slickslider.yaml` to `user/config/plugins/slickslider.yaml` and only edit that copy.

Here is the default configuration and an explanation of available options:

```yaml
enabled: true
slidesToShow: 1
fade: true
autoplaySpeed: 4000
speed: 2000
```

Note that if you use the Admin Plugin, you can set all these Options from there, including some explanation. Having done that, a file with your configuration named slickslider.yaml will be saved in the `user/config/plugins/`-folder once the configuration is saved in the Admin.

## Usage

You can add a nice Picture Slider to any Page in your Grav Site by just adding a shortcode somewhere in your Page's .md File,
e.g. ```[slickslider imgFiles="/slider-demo/slides/img1.jpg,/slider-demo/slides/img2.jpg,/slider-demo/slides/img3.jpg"][/slickslider]``` where the Image Files (the Slides) must be referred to with specification of the Path relative to your Grav Installation - in the Example shown above, the Image Files (Slides) are located in http://yoursite.com/slider-demo/slides .

## Credits

This Plugin is based on Ken Wheeler's [Slick Slider](https://github.com/kenwheeler/slick).

## To Do

- [ ] currently nothing :-)

