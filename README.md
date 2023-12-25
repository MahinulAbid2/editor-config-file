# .editorconfig
editor config file is a text file which helps configure the editor code writing style <br>
This repository is a knowledge combining my note khata and this repo. <br>
In this repo, many information are missing because they are on my khata.

<br>
<br>


## Comments on `.editorconfig`
* I can use comments in .editorconfig file.
* Anything that start with ` # ` becomes a `single-line-comment`

<br>
<br>

| Key  | Value                     | Description                                             |
| ------ | ------------------------- | ------------------------------------------------------|
| root | true or false             | meaning: is this the main configuration file for this project? If yes then overwrite all other rules. |
| charset | utf-8, utf-8-bom, utf-16be, utf-16le            | encoding of that file. |
| indent_style | tab or space    | set to tab or space to use hard tabs or soft tabs respectively. |
| trim_trailing_whitespace | true or false   | set to true to remove any whitespace characters preceding newline characters and false to ensure it doesn't. |
| insert_final_newline | true or false   | set to true to ensure file ends with a newline when saving and false to ensure it doesn't. |

<br>
<br>

### If I forget about indentation.
Google about `what is indentation?`, `what is space and tab indentation`,


<br>
<br>


```
# Top-most EditorConfig file
root = true

# selecting every file with [*]
[*]
charset = utf-8
end_of_line = lf
insert_final_newline = true
trim_trailing_whitespace = true
max_line_length = 80

# selecting only file that has .js extension.
# even if I set all file [*] rules, when I specify a file type it will override [*]
[*.js]
indent_style = space
indent_size = 2

[*.ts]
indent_style = space
indent_size = 2

# Python files
[*.py]
indent_style = space
indent_size = 4

# HTML files
[*.html]
indent_style = space
indent_size = 4


```
