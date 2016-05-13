# Disable Feature UI

Feature 1.x is unsupported, but quite a lot of hassle to remove from our
projects. To prevent security issues we simple disable the full UI of Features,
because we hardly ever use that. 

## Usage

Add this to your `.make` file.

```
projects[disable_features_ui][type]                         = "module"
projects[disable_features_ui][download][type]               = "git"
projects[disable_features_ui][download][url]                = "git@github.com:hoppinger/drupal-disable_features_ui.git"
projects[disable_features_ui][subdir]                       = "hoppinger"
projects[disable_features_ui][subdir]                       = "disable_features_ui"
```
