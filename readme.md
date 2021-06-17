# Warren Shea's "Stranded on a Desert Island Web Development Tools" - Configuration Settings, Packages, Chrome Extensions

## Sublime Text 4 (Registered)

### Packages
* https://packagecontrol.io/packages/Package Control
* https://packagecontrol.io/packages/HTML-CSS-JS Prettify
* https://packagecontrol.io/packages/Increment Selection
  * CTRL + ALT + I
  * CMD + CRTL + I
* https://packagecontrol.io/packages/HTML Minifier
* https://packagecontrol.io/packages/Origami
* https://packagecontrol.io/packages/RainbowBrackets
* https://packagecontrol.io/packages/BracketHighlighter

### Configuration Settings
```json
{
  "auto_complete_commit_on_tab": false,
  "auto_match_enabled": false,
  "color_scheme": "Packages/Color Scheme - Default/Monokai.sublime-color-scheme",
  "folder_exclude_patterns":
  [
    ".svn",
    ".git",
    ".hg",
    "CVS",
    "_site",
    "node_modules",
    "resources",
    "_dist"
  ],
  "font_size": 11,
  "ignored_packages":
  [
    "SublimeLinter-csslint",
    "Vintage"
  ],
  "tab_completion": false,
  "tab_size": 2,
  "theme": "Adaptive.sublime-theme",
  "translate_tabs_to_spaces": true,
  "word_wrap": false,
  "trim_trailing_white_space_on_save": true
}
```
## Python 3

### Packages
* beautifulsoup4
* bs4
* pip
* requests
* selenium
* xlsxWriter

## Chrome

### Extensions
* Pesticide

## Mac OSX
* Karabiner Elements
```
"rules": [
    {
        "description": "Home to Command Left",
        "manipulators": [{
                "from": { "key_code": "home" },
                "to": [ { "key_code": "left_arrow", "modifiers": ["left_command"] }],
                "type": "basic"
        }]
    },
    {
        "description": "Home to Command Left (SHIFT VERSION)",
        "manipulators": [{
                "from": { "key_code": "home", "modifiers": { "mandatory": [ "left_shift" ]}},
                "to": [{ "key_code": "left_arrow", "modifiers": ["left_command","left_shift"] }],
                "type": "basic"
        }]
    },
    {
        "description": "Home to Command Up",
        "manipulators": [{
                "from": { "key_code": "home", "modifiers": { "mandatory": [ "left_command" ]}},
                "to": [{ "key_code": "up_arrow", "modifiers": ["left_command"] }],
                "type": "basic"
        }]
    },
    {
        "description": "Home to Command Up (SHIFT VERSION)",
        "manipulators": [{
                "from": { "key_code": "home", "modifiers": { "mandatory": [ "left_command", "left_shift" ]}},
                "to": [ { "key_code": "up_arrow", "modifiers": ["left_command","left_shift"] }],
                "type": "basic"
        }]
    },
    {
        "description": "End to Command Left",
        "manipulators": [{
                "from": { "key_code": "end" },
                "to": [{ "key_code": "right_arrow", "modifiers": ["left_command"] }],
                "type": "basic"
        }]
    },
    {
        "description": "End to Command Left (SHIFT VERSION)",
        "manipulators": [{
                "from": { "key_code": "end", "modifiers": { "mandatory": [ "left_shift" ]}},
                "to": [{ "key_code": "right_arrow", "modifiers": ["left_command","left_shift"] }],
                "type": "basic"
        }]
    },
    {
        "description": "End to Command Down",
        "manipulators": [{
                "from": { "key_code": "end", "modifiers": { "mandatory": [ "left_command" ]}},
                "to": [{ "key_code": "down_arrow", "modifiers": ["left_command"] }],
                "type": "basic"
        }]
    },
    {
        "description": "End to Command Down (SHIFT VERSION)",
        "manipulators": [{
                "from": { "key_code": "end", "modifiers": { "mandatory": [ "left_command", "left_shift" ]}},
                "to": [{ "key_code": "down_arrow", "modifiers": ["left_command","left_shift"] }],
                "type": "basic"
        }]
    }
]
```
* iTerm2 + Oh My ZSH
  * bullet-train-custom.zsh-theme
  * .zshrc
    * ZSH_THEME = "bullet-train-custom"
    * Font - Menlo + Select Use built-in powerline gylph
* Transmit 5
