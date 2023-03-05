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
* https://packagecontrol.io/packages/RegReplace

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

### RegReplace
Deafult (OSX).sublime-keymap
```json
{
    "replacements": {
        "rule_1": {
            "find": "ABC",
            "replace": "XYZ",
            "greedy": true
        },
        "rule_2": {
            "find": "DEF",
            "replace": "ABCD",
            "greedy": true
        }
    }
}
```

reg_replace_rules.sublime-settings
```json
[
    {
        "keys": ["option+command+r"],
        "command": "reg_replace",
        "args": {"replacements": ["rule_1","rule_2"]}
    }
]
```

## Python 3

### Packages
* beautifulsoup4
* bs4
* pip
* requests
* selenium
* xlsxWriter

## Cmder
```txt
>""C:\Program Files\Git\bin\sh.exe" --login -i" -new_console:d:"E:\local\warrenshea.github.io-dev":t:"Commits" -cur_console:n
""C:\Program Files\Git\bin\sh.exe" --login -i" -new_console:d:"E:\local\warrenshea.github.io-dev":t:"Local Environment" -cur_console:s1TVn
""C:\Program Files\Git\bin\sh.exe" --login -i" -new_console:d:"E:\local\warrenshea.github.io-dev\_dev\notes\":t:"Notes" -cur_console:s1THn
""C:\Program Files\Git\bin\sh.exe" --login -i" -new_console:d:"E:\local\":t:"Other" -cur_console:s2TVn
""C:\Program Files\Git\bin\sh.exe" --login -i" -new_console:d:"E:\local\":t:"Other" -cur_console:s2THn
""C:\Program Files\Git\bin\sh.exe" --login -i" -new_console:d:"E:\local\warrenshea.github.io\":t:"Prod" -cur_console:s3TVn
```

## Chrome

### Settings
Settings > Perferences > Elements > [x] Show user agent shadow DOM

### Extensions
* Pesticide
* Stylus
* Web Developer

## Mac OSX
* Karabiner Elements
/Users/$USERNAME/.config/karabiner/karabiner.json
```
"rules": [
    {
        "description": "Home to Command Left",
        "manipulators": [{
                "from": { "key_code": "home" },
                "to": [ { "key_code": "left_arrow", "modifiers": ["left_command"] }],
                "type": "basic",
                "conditions": [{
                    "bundle_identifiers": ["^com\\.apple\\.Terminal$","^com\\.googlecode\\.iterm2$","^com\\.sublimetext\\.3$","^com\\.sublimetext\\.4\\.plist$"],
                    "type": "frontmost_application_unless"
                }
            ]
        }]
    },
    {
        "description": "Home to Command Left (SHIFT VERSION)",
        "manipulators": [{
                "from": { "key_code": "home", "modifiers": { "mandatory": [ "left_shift" ]}},
                "to": [{ "key_code": "left_arrow", "modifiers": ["left_command","left_shift"] }],
                "type": "basic",
                "conditions": [{
                    "bundle_identifiers": ["^com\\.apple\\.Terminal$","^com\\.googlecode\\.iterm2$","^com\\.sublimetext\\.3$","^com\\.sublimetext\\.4\\.plist$"],
                    "type": "frontmost_application_unless"
                }
            ]
        }]
    },
    {
        "description": "Home to Command Up",
        "manipulators": [{
                "from": { "key_code": "home", "modifiers": { "mandatory": [ "left_command" ]}},
                "to": [{ "key_code": "up_arrow", "modifiers": ["left_command"] }],
                "type": "basic",
                "conditions": [{
                    "bundle_identifiers": ["^com\\.apple\\.Terminal$","^com\\.googlecode\\.iterm2$","^com\\.sublimetext\\.3$","^com\\.sublimetext\\.4\\.plist$"],
                    "type": "frontmost_application_unless"
                }
            ]
        }]
    },
    {
        "description": "Home to Command Up (SHIFT VERSION)",
        "manipulators": [{
                "from": { "key_code": "home", "modifiers": { "mandatory": [ "left_command", "left_shift" ]}},
                "to": [ { "key_code": "up_arrow", "modifiers": ["left_command","left_shift"] }],
                "type": "basic",
                "conditions": [{
                    "bundle_identifiers": ["^com\\.apple\\.Terminal$","^com\\.googlecode\\.iterm2$","^com\\.sublimetext\\.3$","^com\\.sublimetext\\.4\\.plist$"],
                    "type": "frontmost_application_unless"
                }
            ]
        }]
    },
    {
        "description": "End to Command Left",
        "manipulators": [{
                "from": { "key_code": "end" },
                "to": [{ "key_code": "right_arrow", "modifiers": ["left_command"] }],
                "type": "basic",
                "conditions": [{
                    "bundle_identifiers": ["^com\\.apple\\.Terminal$","^com\\.googlecode\\.iterm2$","^com\\.sublimetext\\.3$","^com\\.sublimetext\\.4\\.plist$"],
                    "type": "frontmost_application_unless"
                }
            ]
        }]
    },
    {
        "description": "End to Command Left (SHIFT VERSION)",
        "manipulators": [{
                "from": { "key_code": "end", "modifiers": { "mandatory": [ "left_shift" ]}},
                "to": [{ "key_code": "right_arrow", "modifiers": ["left_command","left_shift"] }],
                "type": "basic",
                "conditions": [{
                    "bundle_identifiers": ["^com\\.apple\\.Terminal$","^com\\.googlecode\\.iterm2$","^com\\.sublimetext\\.3$","^com\\.sublimetext\\.4\\.plist$"],
                    "type": "frontmost_application_unless"
                }
            ]
        }]
    },
    {
        "description": "End to Command Down",
        "manipulators": [{
                "from": { "key_code": "end", "modifiers": { "mandatory": [ "left_command" ]}},
                "to": [{ "key_code": "down_arrow", "modifiers": ["left_command"] }],
                "type": "basic",
                "conditions": [{
                    "bundle_identifiers": ["^com\\.apple\\.Terminal$","^com\\.googlecode\\.iterm2$","^com\\.sublimetext\\.3$","^com\\.sublimetext\\.4\\.plist$"],
                    "type": "frontmost_application_unless"
                }
            ]
        }]
    },
    {
        "description": "End to Command Down (SHIFT VERSION)",
        "manipulators": [{
                "from": { "key_code": "end", "modifiers": { "mandatory": [ "left_command", "left_shift" ]}},
                "to": [{ "key_code": "down_arrow", "modifiers": ["left_command","left_shift"] }],
                "type": "basic",
                "conditions": [{
                    "bundle_identifiers": ["^com\\.apple\\.Terminal$","^com\\.googlecode\\.iterm2$","^com\\.sublimetext\\.3$","^com\\.sublimetext\\.4\\.plist$"],
                    "type": "frontmost_application_unless"
                }
            ]
        }]
    }
]
```
* iTerm2 + Oh My ZSH
  * /Users/&lt;username&gt;/.oh-my-zsh/themes/[bullet-train-custom.zsh-theme](bullet-train-custom.zsh-theme)
  * /Users/&lt;username&gt;/.zshrc
    * ZSH_THEME = "bullet-train-custom"
    * Font - Menlo + Select Use built-in powerline gylph

* ChromeDriver
  * /user/local/bin/chromedriver

* Transmit 5
