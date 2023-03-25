# Sublime Text 3 Path Copy Plugin

Sublime Text plugin to add path copying commands to the Command Palette and right-click context menu.

General files:

* Copy the path of the current file.
* Copy the name of the current file.
* Copy the directory of the current file.
* Copy the path of the current file relative to its project's root directory.
* Copy the directory of the current file relative to its project's root directory.

C/C++ files:

* Copy the path of the current file relative to its project's root directory as a C/C++ `#include` macro.
* Copy the path of the current file relative to its project's root directory as an Objective-C/C++ `#import` macro.
* Copy the path of the current file relative to its project's root directory as a C/C++ header guard.

Java files:

* Copy the path of the current file relative to its project's root directory as a Java import statement.
* Copy the directory of the current file relative to its project's root directory as a Java package statement.

## Settings

This plugin may be configured via [project settings](https://www.sublimetext.com/docs/3/projects.html).
The following settings may be used:

```json
{
    "folders": [],
    "settings": {
        "copy-paths": {
            "c_family_includes_use_brackets": true,
        }
    }
}
```

* `c_family_includes_use_brackets` - If enabled, copying the current file as a `#include` or `#import`
   macro will do so with angle brackets (`<` and `>`). Otherwise, defaults to using quotation marks.
