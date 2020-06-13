# Warning

This repository is a fork of [the original Better Comments](https://github.com/aaron-bond/better-comments). It adds support for TLA+ and fixes some minor issues.

Builds of the extension from this repository are not published on VS Code Marketplace. But you can grab them from the [Releases page](https://github.com/alygin/better-comments/releases) and [install .vsix files manually](https://code.visualstudio.com/docs/editor/extension-gallery#_install-from-a-vsix).

# Better Comments

The Better Comments extension will help you create more human-friendly comments in your code.  
With this extension, you will be able to categorise your annotations into:
* Alerts
* Queries
* TODOs
* Highlights
* Commented out code can also be styled to make it clear the code shouldn't be there
* Any other comment styles you'd like can be specified in the settings

<img src="https://raw.githubusercontent.com/alygin/better-comments/master/images/better-comments.PNG" width="459" height="auto">

## Configuration

This extension can be configured in User Settings or Workspace settings.


`"better-comments.multilineComments": true`  
 This setting will control whether multiline comments are styled using the annotation tags.
 When false, multiline comments will be presented without decoration.

`"better-comments.highlightPlainText": false`  
This setting will control whether comments in a plain text file are styled using the annotation tags.
When true, the tags (defaults: `! * ? //`) will be detected if they're the first character on a line.

`better-comments.tags`  
The tags are the characters or sequences used to mark a comment for decoration.
The default 5 can be modifed to change the colors, and more can be added.
```json
"better-comments.tags": [
  {
    "tag": "!",
    "color": "#FF2D00",
    "strikethrough": false,
    "backgroundColor": "transparent"
  },
  {
    "tag": "?",
    "color": "#3498DB",
    "strikethrough": false,
    "backgroundColor": "transparent"
  },
  {
    "tag": "//",
    "color": "#474747",
    "strikethrough": true,
    "backgroundColor": "transparent"
  },
  {
    "tag": "todo",
    "color": "#FF8C00",
    "strikethrough": false,
    "backgroundColor": "transparent"
  },
  {
    "tag": "*",
    "color": "#98C379",
    "strikethrough": false,
    "backgroundColor": "transparent"
  }
]
```

## Supported Languages

* Ada
* AL
* Apex
* AsciiDoc
* C
* C#
* C++
* ColdFusion
* Clojure
* COBOL
* CoffeeScript
* CSS
* Dart
* Dockerfile
* Elixir
* Elm
* Erlang
* F#
* Fortran
* gdscript
* GenStat
* Go
* GraphQL
* Groovy
* Haskell
* Haxe
* HiveQL
* HTML
* Java
* JavaScript
* JavaScript React
* JSON with comments
* Julia
* Kotlin
* LaTex (inlc. Bibtex/Biblatex)
* Less
* Lisp
* Lua
* Makefile
* Markdown
* Nim
* MATLAB
* Objective-C
* Objective-C++
* Pascal
* Perl
* Perl 6
* PHP
* Pig
* PlantUML
* PL/SQL
* PowerShell
* Puppet
* Python
* R
* Racket
* Ruby
* Rust
* SAS
* Sass
* Scala
* SCSS
* ShaderLab
* ShellScript
* SQL
* STATA
* Stylus
* Swift
* Tcl
* Terraform
* Twig
* TypeScript
* TypeScript React
* Verilog
* Visual Basic
* Vue.js
* YAML
