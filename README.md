# Find++

Find code quickly in [Sublime Text][subl].

This was built to allow quick shuffling between search directories. It is useful for projects using multiple repositories to isolate noise in search results.

[subl]: http://www.sublimetext.com/

- `Find: In Current File` - Opens `Find in Files` with `Where` as the current file
- `Find: In Current Folder` - Opens `Find in Files` with `Where` as the folder of the current file
- `Find: In Open Files` - Opens `Find in Files` with `Where` as `<open files>`
- `Find: In Project` - Opens `Find in Files` with `Where` as `<open files>,<open folders>`
- `Find: In...` - Shows panel to pick directory to open `Find in Files` with as its `Where`
- `Find: Show Results Panel` - Reveals the `Find Results` panel

![Find in Files example](https://f.cloud.github.com/assets/902488/860977/39331c12-f5c2-11e2-9de7-9769e885d111.png)


## Installation

### By Package Control

1. Download & Install **`Sublime Text 3`** (https://www.sublimetext.com/3)
1. Go to the menu **`Tools -> Install Package Control`**, then,
   wait few seconds until the installation finishes up
1. Now,
   Go to the menu **`Preferences -> Package Control`**
1. Type **`Add Channel`** on the opened quick panel and press <kbd>Enter</kbd>
1. Then,
   input the following address and press <kbd>Enter</kbd>
   ```
   https://raw.githubusercontent.com/evandrocoan/StudioChannel/master/channel.json
   ```
1. Go to the menu **`Tools -> Command Palette...
   (Ctrl+Shift+P)`**
1. Type **`Preferences:
   Package Control Settings – User`** on the opened quick panel and press <kbd>Enter</kbd>
1. Then,
   find the following setting on your **`Package Control.sublime-settings`** file:
   ```js
       "channels":
       [
           "https://packagecontrol.io/channel_v3.json",
           "https://raw.githubusercontent.com/evandrocoan/StudioChannel/master/channel.json",
       ],
   ```
1. And,
   change it to the following, i.e.,
   put the **`https://raw.githubusercontent...`** line as first:
   ```js
       "channels":
       [
           "https://raw.githubusercontent.com/evandrocoan/StudioChannel/master/channel.json",
           "https://packagecontrol.io/channel_v3.json",
       ],
   ```
   * The **`https://raw.githubusercontent...`** line must to be added before the **`https://packagecontrol.io...`** one, otherwise,
     you will not install this forked version of the package,
     but the original available on the Package Control default channel **`https://packagecontrol.io...`**
1. Now,
   go to the menu **`Preferences -> Package Control`**
1. Type **`Install Package`** on the opened quick panel and press <kbd>Enter</kbd>
1. Then,
search for **`Find++`** and press <kbd>Enter</kbd>

See also:

1. [ITE - Integrated Toolset Environment](https://github.com/evandrocoan/ITE)
1. [Package control docs](https://packagecontrol.io/docs/usage) for details.


## Documentation
All commands are accessible via the Command Palette, `Ctrl + Shift + P` on Windows/Linux, `Command + Shift + P` on Mac.

![Find Palette](https://f.cloud.github.com/assets/902488/279674/a552365a-9134-11e2-8c89-603fbb89b606.png)

The `Find: In...` command opens a quick panel with relevant paths and the ability to filter.

![Find in current file panel](https://f.cloud.github.com/assets/902488/860987/ba97f2b4-f5c2-11e2-9b8d-c53060cd0f59.png)

When you search, the normal `Find in Files` search will be executed with one modification. The `Delete` and `Backspace` key will delete an entire row rather than a single character.

![Find in files results](https://f.cloud.github.com/assets/902488/279676/acdae412-9134-11e2-9c3d-10cdaaa6daff.png)

## Donating
Support this project and [others by twolfson][twolfson-projects] via [donations][twolfson-support-me].

<http://twolfson.com/support-me>

[twolfson-projects]: http://twolfson.com/projects
[twolfson-support-me]: http://twolfson.com/support-me

## Inspiration
As the name of this project suggests, this plugin was started to gain the same `Find` functionality of [Notepad++][npp].

[npp]: http://notepad-plus-plus.org/

## License
Copyright (c) 2013 Todd Wolfson

Licensed under the MIT license.
