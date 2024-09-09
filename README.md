# SublimeRelated
A repository where I store settings, packages, and files in regards to my SublimeText setup.   

Path:   
C:\Users\admin\AppData\Roaming\Sublime Text\Packages\User   

## PACKAGES

1. SublimeTmpl   
2. ANSIescape   
3. ColorHelper   
4. A File Icon   
5. FavoriteFiles   
6. Increment Selection   
7. LiveServer   
8. MarkdownPreview   
9. nginx   
10. Origami   
11. BuildView   
12. BuildX   
13. Terminus   

## Key bindings
// Default (Windows.sublime-keymap)
```json
[
{
  "keys": ["ctrl+b"],
  "command": "build",
  "context": [{"key": "for_buildx", "operator":"equal", "operand":true}]
},
{
  "keys": ["ctrl+shift+b"],
  "command": "build",
  "args": {"select": true},
  "context": [{"key": "for_buildx", "operator":"equal", "operand":true}]
},

  {
    "keys": ["ctrl+shift+c"], // Replace with your preferred key binding
    "command": "terminus_cancel_build"
  },
  
  { 
    "keys": ["ctrl+alt+c"], "command": "toggle_comment", "args": { "block": false } 
  },
  
  { 
    "keys": ["ctrl+alt+c"], "command": "toggle_comment", "args": { "block": true } 
  },
]

```

## packages settings   
### BuildX
```json
{
  "process_ansi_color": true,
  "preserve_content": true,
  "clear_output_when_build_starts": false,
  "ansi_color": {
    "bg": "#292d3e",
    "fg": "#abb2bf",
    "block_caret": "#515562",
    "caret": "#515562",
    "gutter": "#292d3e",
    "gutter_foreground": "#3a3f58",
    "invisibles": "#ffffff33",
    "line_highlight": "#ffffff00",
    "selection": "#ffffff11",
    "black": "#545862",
    "red": "#e06c75",
    "green": "#98c379",
    "yellow": "#e5c07b",
    "blue": "#61afef",
    "magenta": "#c678dd",
    "cyan": "#56b6c2",
    "white": "#ddd",
    "bright_black": "#545862",
    "bright_white": "#c8ccd4",
    "bright_red": "#e06c75",
    "bright_green": "#98c379",
    "bright_yellow": "#e5c07b",
    "bright_blue": "#61afef",
    "bright_magenta": "#c678dd",
    "bright_cyan": "#56b6c2"
  },
  "syntax_color": {
    "success_msg": "#98c379",
    "success_time": "#ccc",
    "error_msg": "#e06c75",
    "error_time": "#ccc",
    "error_code": "#e5c07b"
  }
}

```

### SublimeTmpl
```json
{
    "html": {
        "syntax": "Packages/HTML/HTML.tmLanguage",
        "extension": "html" // default_extension
    },
    "js": {
        "syntax": "Packages/JavaScript/JavaScript.tmLanguage",
        "extension": "js"
    },
    "css": {
        "syntax": "Packages/CSS/CSS.tmLanguage",
        "extension": "css"
    },
    "xml": {
        "syntax": "Packages/XML/XML.tmLanguage",
        "extension": "xml"
    },
    "php": {
        "syntax": "Packages/PHP/PHP.tmLanguage",
        "extension": "php"
    },
    "java": {
        "syntax": "Packages/Java/Java.tmLanguage",
        "extension": "java"
    },
    "ruby": {
        "syntax": "Packages/Ruby/Ruby.tmLanguage",
        "extension": "rb"
    },
    "python": {
        "syntax": "Packages/Python/Python.tmLanguage",
        "extension": "py"
    },
    "objective-c": {
        "syntax": "Packages/Objective-C/Objective-C.tmLanguage",
        "extension": "m"
    },
    "c++": {
        "syntax": "Packages/C++/C++.tmLanguage",
        "extension": "cpp"
    },
    "C#": {
        "syntax": "Packages/C#/C#.tmLanguage",
        "extension": "cs"
    },
    "Perl": {
        "syntax": "Packages/Perl/Perl.tmLanguage",
        "extension": "pl"
    },
    "sass": {
        "syntax": "Packages/SCSS/SCSS.tmLanguage",
        // "syntax": "Packages/Sass/Syntaxes/Sass.tmLanguage",
        "extension": "scss"
    },
    "go": {
        "syntax": "Packages/Go/Go.tmLanguage",
        "extension": "go"
    },
    "groovy": {
        "syntax": "Packages/Groovy/Groovy.tmLanguage",
        "extension": "groovy"
    },
    "erlang": {
        "syntax": "Packages/Erlang/Erlang.tmLanguage",
        "extension": "erl"
    },
    "jade": {
        "syntax": "Packages/Jade/Syntaxes/Jade.tmLanguage",
        "extension": "jade"
    },
    "less": {
        "syntax": "Packages/LESS/LESS.tmLanguage",
        "extension": "less"
    },
    "lisp": {
        "syntax": "Packages/Lisp/Lisp.tmLanguage",
        "extension": "lisp"
    },
    "lua": {
        "syntax": "Packages/Lua/Lua.tmLanguage",
        "extension": "lua"
    },
    "make": {
        "syntax": "Packages/Makefile/Makefile.tmLanguage",
        "extension": "make"
    },
    "rust": {
        "syntax": "Packages/Rust/Rust.tmLanguage",
        "extension": "rs"
    },
    "scala": {
        "syntax": "Packages/Scala/Scala.tmLanguage",
        "extension": "scala"
    },
    "shellscript": {
        "syntax": "Packages/ShellScript/Shell-Unix-Generic.tmLanguage",
        "extension": "sh"
    },
    "sql": {
        "syntax": "Packages/SQL/SQL.tmLanguage",
        "extension": "sql"
    },
    "yaml": {
        "syntax": "Packages/YAML/YAML.tmLanguage",
        "extension": "yaml"
    },
    "disable_keymap_actions": false, // "all"; "html,css"
    "enable_project_variables": false,
    "enable_file_variables_on_save": false,
    "date_format" : "%Y-%m-%d %H:%M:%S",
    "attr": {
        "author": "JML",
        "email": "jockemedlinux@gmail.com",
        "link": "https://jockemedlinux.dev"
    },
    "project_variables": {
        // Allows for use with other template formats, provide mapping here
        // "tmpl_formatted_name": "current_template_name"
        "project_base_name": "project_base_name",
        "project_path": "project_path",
        "platform": "platform"
    },
    
    "file_variables_on_save": {
        // Allows for use with other template formats, provide mapping here
        // "tmpl_formatted_name": "current_template_name"
        "saved_filename": "saved_filename",
        "saved_filepath": "saved_filepath"
    },
    "template_replace_pattern": "${%s}",
    "template_extension": ".tmpl"
}
```

### Terminus
// jml.sublime-build
```json
{
  "target": "terminus_open",
  "title": "Python Output [jml]",
  "cmd": ["python", "-u", "$file"],
  "cwd": "${file_path}",
  "working_dir": "${file_path}",
  "auto_close": false,
  "focus": true,
  "panel_name": "python_output",
  "pre_window_hooks": [
    ["move_to_pane", {"direction": "right"}]
  ]
}
```

## snippets 

///codeblock-py.sublime-snippet
```xml
<snippet>
	<content><![CDATA[
```py
$SELECTION

]]></content>
	<!-- Optional: Set a tabTrigger to define how to trigger the snippet -->
	<!-- <tabTrigger>hello</tabTrigger> -->
	<!-- Optional: Set a scope to limit where the snippet will trigger -->
	<!-- <scope>source.python</scope> -->
</snippet>

```

// colors.sublime-snippet
```xml
<snippet>
	<content><![CDATA[
class colors:
    MAGENTA = '\033[95m'            
    BLUE = '\033[94m'               
    CYAN = '\033[96m'               
    GREEN = '\033[92m'              
    ORANGE = '\033[93m'        
    YELLOW='\033[0;33m'
    RED = '\033[91m'                
    BLACK = '\033[0;30m'        
    PURPLE = '\033[0;35m'       
    WHITE = '\033[0;37m'        
    RESET = '\033[0m'

]]></content>
	<!-- Optional: Set a tabTrigger to define how to trigger the snippet -->
	<!-- <tabTrigger>hello</tabTrigger> -->
	<!-- Optional: Set a scope to limit where the snippet will trigger -->
	<!-- <scope>source.python</scope> -->
</snippet>

```