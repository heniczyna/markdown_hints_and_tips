# Links
[Info](<https://agea.github.io/tutorial.md/>)<br>
[Relative links and image paths in README files](<https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes#relative-links-and-image-paths-in-readme-files>)

| comments                                                      | source                                | output                              |
|---------------------------------------------------------------|---------------------------------------|-------------------------------------|
| in `<>` brackets, use when link contains spaces               | `[google](<https://www.google.com/>)` | [google](<https://www.google.com/>) |
| relative                                                      | `[text1](/texts/text1.txt)`           | [text1](/texts/text1.txt)           |

# Emoji
[Info](<https://stackoverflow.com/questions/48331389/github-markdown-is-it-possible-to-put-links-under-emojis>)

| comments                                                      | source                                | output                              |
|---------------------------------------------------------------|---------------------------------------|-------------------------------------|
| emoji as a link to www                                        | `[:memo:](https://www.google.com/)`   | [:memo:](https://www.google.com/)   |
| emoji as a link to www (paste icon instead of shortcode)      | `[📝](https://www.google.com/)`       | [📝](https://www.google.com/)       |
| emoji as a email address                                      | `[:black_nib:](mailto:person@ex.com)` | [:black_nib:](mailto:person@ex.com) |
| emoji as a email address (paste icon instead of shortcode)    | `[✒️](mailto:person@ex.com)`          | [✒️](mailto:person@ex.com)          |

Emoji icons copied from [here](<https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md>)

> **Additional info**
> * when publishing the repo using GitHub Pages, emoji icons are not rendered properly, you will only see `:memo:` instead of icon


# Comments
Seems comments do not work in table.

`<!--- line I do not want to be placed in markdown document --->`. And below the same line without ` `` ` markups which you should not be able to see 😄

<!--- line I do not want to be placed in markdown document --->

# Tables
[Markdown Table Generator](<https://www.tablesgenerator.com/markdown_tables>)

# Images
| comments                               | source                                                    | output                                                   |
|----------------------------------------|-----------------------------------------------------------|----------------------------------------------------------|
| relative link, to image in this repo (**this should be preferred, i.e. without `/` at the begining, based on [GitHub doc](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes#relative-links-and-image-paths-in-readme-files)**) | `![stopwatch_224x272.bmp](images/stopwatch_224x272.bmp)`  | ![stopwatch_224x272.bmp](images/stopwatch_224x272.bmp) |
| `/images` instead of `images`, also works | `![stopwatch_224x272.bmp](/images/stopwatch_224x272.bmp)` | ![stopwatch_224x272.bmp](/images/stopwatch_224x272.bmp) |
| `images` and hyperlink | `[![stopwatch_224x272.bmp](images/stopwatch_224x272.bmp)](https://www.google.com/)` | [![stopwatch_224x272.bmp](images/stopwatch_224x272.bmp)](https://www.google.com/) |

# Additional info
**source**
```
> **Additional info**
> * info you would like to highlight
```
**output**
> **Additional info**
> * info you would like to highlight

# Code syntax highlighting
[Info](<https://support.codebasehq.com/articles/tips-tricks/syntax-highlighting-in-markdown>)

**source**<br>
Change ` ``cpp ` to ` ```cpp ` and ` `` ` to ` ``` `
```
``cpp
int main(){}
return 0;
``
```
**output for *cpp***
```cpp
int main(){}
return 0;
```
**output for *console***
```console
xxd -version
```

# Line break
**source**
```
And now I want to put break<br>
and go further.
```
**output**<br>
And now I want to put break<br>
and go further.

**Comparison to double `Enter`**

**source**
```
And now I want to put break

and go further.
```
**output**<br>
And now I want to put break

and go further.

The space between the lines when using double `Enter` is to much in this case. Therefore, `<br` is required sometimes. However, I do not know whether this is recommended way or not.

# File names
* as a code within ` `` ` markups: `/board/pin_mux.h`
* when creating next markdown document try with `*`: */board/pin_mux.h* and leave the code markups for code?
* or use italics only with name such as *pin_mux.h* (I have seen that in some GitHub doc) and use code markups when providing also directory such as `/board/pin_mux.h`?
* some suggestions from [SO](<https://meta.stackexchange.com/questions/246900/which-markdown-formatting-should-be-used-for-a-filename-of-code>)
#### **`hello_world.js`**
``` js
alert("Hello world!");
```
> **test.bat**
> ```
> @echo off
> echo %~1
> ```

# Hit/choose an option
* as a code within ` `` ` markups: From `QuickStart Panel` choose `Import`
* as bold text?: From **QuickStart Panel** choose **Import**

# Indentation in lists containing the code
Add indentation to code (3 or 4 spaces, to double-check, make it aligned with *Open* word), to align the code with element of the list. As below, code block is aligned with first element of the list.
1. Open **Command Prompt** with **cmd** and convert model to **.h* array with command:
   ```console
   xxd -i ssd_mobilenet_v1_1_metadata_1.tflite > ssd_mobilenet_v1_1_metadata_1.h
   ```
   * *xxd* is part of [*Vim*](https://www.vim.org/) text editor
   * if `xxd -version` does not work straight away after *Vim* installation, please double check *Vim* installation directory
2. Move converted ...


