# lint-auto-fix
Save action: automatically fix ESLint errors

# Initial Project Setup

`npm init`

`npm install eslint --save-dev`

### ESLint

https://eslint.org/docs/user-guide/getting-started

`.\node_modules\.bin\eslint --init`

- How would you like to configure ESLint? Answer questions about your style
- Are you using ECMAScript 6 features? Yes
- Are you using ES6 modules? Yes
- Where will your code run? Browser
- Do you use CommonJS? No
- Do you use JSX? Yes
- Do you use React? Yes
- What style of indentation do you use? Tabs
- What quotes do you use for strings? Single
- What line endings do you use? Unix
- Do you require semicolons? Yes
- What format do you want your config file to be in? JSON

# Links

Markdown
- [GitHub-Flavored-Markdown-(GFM)-language-IDs](https://github.com/jmm/gfm-lang-ids/wiki/GitHub-Flavored-Markdown-(GFM)-language-IDs)

Husky etc.
- https://www.google.ch/search?q=husky+js&oq=husky+js&aqs=chrome..69i57.1207j0j4&sourceid=chrome&ie=UTF-8
- https://davidwalsh.name/prevent-bad-commits-husky
- https://github.com/typicode/husky
- https://github.com/typicode/husky/tree/dev
- https://www.google.ch/search?q=fix+lint+error+on+save+intellij&oq=fix+lint+error+on+save+intellij&aqs=chrome..69i57.14599j0j7&sourceid=chrome&ie=UTF-8
- https://intellij-support.jetbrains.com/hc/en-us/community/posts/115000221130-Eslint-autofix-on-save-for-webstorm
- https://youtrack.jetbrains.com/issue/WEB-24452#comment=27-1763733&u=1480596291921
- https://youtrack.jetbrains.com/issue/IDEABKL-6722#u=1401303765668
 
# Plugins

- GitToolBox
- Key Promoter X (display ballon tips with keyboard shortcuts for IntelliJ actions)
- SvgViewer 2
- File Watchers

![Plugins](screenshots/24-11-_2017_12-14-31.png)

# External Tools

```
npm run lint-fix
C:\Program Files (x86)\nodejs\npm.cmd
run lint-fix $FilePathRelativeToProjectRoot$
$ProjectFileDir$
```

![ExternalTools](screenshots/26-11-_2017_19-09-18.png)

# Settings

### Appearance & Behavior > Disable "safe write"

![Settings](screenshots/22-11-_2017_09-11-22.png)

### Appearance & Behavior > Disable "check for automatic updates"

![Settings](screenshots/22-11-_2017_09-48-09.png)

### Appearance & Behavior > Disable "usage statistics"

![Settings](screenshots/22-11-_2017_09-51-43.png)

### Editor > General (CamelHumps &rarr; cf. Smart Keys)

![Settings](screenshots/22-11-_2017_10-01-18.png)

### Editor > Code Folding

![Settings](screenshots/22-11-_2017_09-54-36.png)

### Editor > Editor Tabs

![Settings](screenshots/22-11-_2017_09-57-03.png)

### Editor > Smart Keys (CamelHumps &rarr; cf. Editor General)

![Settings](screenshots/22-11-_2017_09-59-17.png)

### Editor > Font

![Settings](screenshots/22-11-_2017_10-08-07.png)

### Editor > Code Style

- Project specific settings &rarr; cf. `<project>/.idea/codeStyleSettings.xml`

![Settings](screenshots/22-11-_2017_10-11-07.png)

### Editor > Code Style > Create file `.editorconfig`

```properties
# EditorConfig is awesome: http://EditorConfig.org

# top-most EditorConfig file
root = true

[*]
charset = utf-8
indent_style = tab
end_of_line = lf
trim_trailing_whitespace = true
insert_final_newline = true

[package.json]
indent_style = space
indent_size = 2

[*.md]
trim_trailing_whitespace = false
```

![Settings](screenshots/22-11-_2017_10-14-17.png)

### Editor > Code Style > JavaScript

![Settings](screenshots/22-11-_2017_18-24-35.png)

### Editor > Code Style > JSON

- Trick for auto-format JSON files &rarr; set 'Right margin (columns)' = 1
- With this trick, the JSON will be nicely formatted on 'Reformat Code (Ctrl Alt L)'
- Hmmmm... this trick seems not to be necessary with IntelliJ 2017.x

```diff
- Does it work on Auto-Save (with Plugin 'Save Actions')??? needs to be tested!!!
```

![Settings](screenshots/22-11-_2017_10-24-23.png)

### Editor > Inspections

```diff
- TODO
```

![Settings](screenshots/)

### Editor > Live Templates

```diff
- TODO
- console.log
```

![Settings](screenshots/)

### Languages & Frameworks > JavaScript

- React JSX (JSX in ECMAScript 6)

![Settings](screenshots/22-11-_2017_12-46-49.png)

### Languages & Frameworks > JavaScript > Code Quality Tools > ESLint

![Settings](screenshots/22-11-_2017_12-51-13.png)

### Languages & Frameworks > Markdown

- jar:file:/C:/Program%20Files/JetBrains/IntelliJ%20IDEA%202017.2.6/plugins/markdown/lib/markdown.jar!/org/intellij/plugins/markdown/settings/default.css
- Markdown Preview Browser: **JavaFX WebView**

![Settings](screenshots/22-11-_2017_13-20-25.png)

![Settings](screenshots/22-11-_2017_13-21-15.png)

### TODO

```diff
- typo (ignore spelling)
```
