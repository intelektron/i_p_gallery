# Gallery paragraph for Droopler #
[![N|Solid](http://intelektron.pl/logo.svg)](http://intelektron.pl)

## Installation ##

1. Update **composer.json**

Put this module in the "require" section of your composer.json. Remember to install required [Colorbox module](https://www.drupal.org/project/colorbox) and [jQuery Colorbox](https://github.com/jackmoore/colorbox) library! I assume you have configured asset-packagist.org and "composer-installers-extender" extension.

```json
"require": {
  "intelektron/i_p_gallery":  "^1.0",
  "drupal/colorbox": "^1.4",
  "npm-asset/jquery-colorbox": "^1.6"
}
```

In the "repositories" section put:

```json
"repositories": {
  "intelektron-gallery": {
    "type": "git",
    "url":  "git@github.com:intelektron/i_p_gallery.git"
  }
}
```

Finally add this to "extra" section as first item in "installer-paths":

```json
"extra": {
  "installer-paths": {
    "web/libraries/colorbox": ["npm-asset/jquery-colorbox"]
  }
}
```

2. Run **composer update**.
3. Enable module in Drupal.
4) Enjoy the new paragraph :-).
