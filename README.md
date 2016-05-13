# Disable Feature UI

Feature 1.x is unsupported, but quite a lot of hassle to remove from our
projects. To prevent security issues we simple disable the full UI of Features,
because we hardly ever use that. 

## Usage for Kraftwagen projects

Add this to your `[PROFILE_NAME].make` file.

```ini
projects[disable_features_ui][type]                         = "module"
projects[disable_features_ui][download][type]               = "git"
projects[disable_features_ui][download][url]                = "git@github.com:hoppinger/drupal-disable_features_ui.git"
projects[disable_features_ui][subdir]                       = "hoppinger"
```

Add this to your `[PROFILE_NAME].info` file.

```ini
env_dependencies[production][] = disable_features_ui
```
