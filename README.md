# Android-Studio-Info



#### Visual Studio Code Shortcuts Keys
- To preview the `Readme.md` file in VSCode -> `Ctrl + Shift + V`
- To format the json document in VSCode -> `Ctrl + K` then `Ctrl + F`
- To format any document, install and then set the **Prettier** extension as the default formatter using `Ctrl + Shift + P`,  
  then format file -> `Shift + Alt + F`

#### Android Studio Shortcuts Keys
- **Reformat** the code in Android Studio -> `Ctrl + Alt + L`
- **Expand** all code blocks in Android Studio -> `Ctrl + Shift + +`
- **Collapse** all code blocks in Android Studio -> `Ctrl + Shift + -`

#### Wireless Debugging Procedure :

- Connect Mobile to 'ICPS 3FL 5GHz' wifi
- Make sure adb is installed on the desktop using the 'adb version' command
- Developer Options -> Wireless Debugging -> Enable -> Pair device with pairing code -> Note the IP, Port, and Pairing Code (changes every time)
- type command in desktop in *sudo* : adb pair <IP>:<Port>
- It asks for a pairing code. Enter pairing code
- If success, then type: adb connect <IP>:<Port>
- adb devices, you can see the connected devices
- Android Studio automatically detects it.

Arial Black
Dialog
Fira Code
Fira Code Medium
HP Simplified
Inter
Inter Semi Bold
Microsoft Sans Serif
Nirmal UI
SansSerif
Verdana



### Duplicating a project
```
cd /home/icps1101/Downloads/projects
cp -r "EasyMarkdown" "TestingMarkdown"
```

Step 2 – Open the Duplicate in Android Studio
In Android Studio:
**File → Open… → Select TestingMarkdown**
Wait for Gradle sync to complete.

Step 3 – Change the Application Name (UI label)
Open: app/src/main/res/values/strings.xml
Edit
```<string name="app_name">Easy Markdown</string>```
Change to:
```<string name="app_name">Testing Markdown</string>```


In the Project view (set to Android mode), expand:

```app/java/com/example/easymarkdown```
Right-click on ```easymarkdown → Refactor → Rename → type testingmarkdown.```

Android Studio will ask if you want to search in comments/strings — check it.

After renaming, open app/build.gradle and update applicationId to match the new package path:

applicationId "com.nithishgajula.testingmarkdown"




<font color='yellow'>**TODO**</font>





# GitHub Flavored Markdown — Feature Showcase

This README demonstrates **all** formatting & features supported by GitHub's own Markdown preview (GFM).

---

## 1. Headings

# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5
###### Heading 6

---

## 2. Text Styling

**Bold text**  
*Italic text*  
***Bold and Italic***  
~~Strikethrough~~  
`Inline code`

---

## 3. Code Blocks




---

## 4. Lists

### Unordered
- Item 1
- Item 2
  - Nested Item 1
  - Nested Item 2

### Ordered
1. First
2. Second
   1. Sub-item
   2. Sub-item

---

## 5. Task Lists

- [x] Completed task
- [ ] Incomplete task
- [ ] Another one

---

## 6. Links and Images

[Visit GitHub](https://github.com)  

![GitHub Logo](https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png)

---

## 7. Tables

| Syntax     | Description |
|------------|-------------|
| Header     | Title       |
| Paragraph  | Text        |

---

## 8. Blockquote

> "GitHub Flavored Markdown is awesome!" — A Developer

---

## 9. Emoji

I :heart: Markdown!  
:rocket: Launching soon!  
:smile: :tada: :+1:

---

## 10. Autolinks

https://github.com  
https://www.google.com

---

## 11. Mentions and References

@octocat  
#1 — Refers to Issue or PR number 1 in the same repo  
octocat/Spoon-Knife#1000 — Cross-repo issue/PR link

---

## 12. Footnotes

Here is a simple footnote[^1].  
A footnote can also have multiple lines[^longnote].

[^1]: My reference.
[^longnote]: Here's one with multiple lines.  
    Indent paragraphs to include them in the footnote.  

    Add as many paragraphs as you like.

---

## 13. Collapsible Sections

<details>
<summary>Click to expand!</summary>

### Hidden Heading
This content is hidden until expanded.


</details>

---

## 14. HTML in Markdown

<kbd>Ctrl</kbd> + <kbd>C</kbd>  
<sup>Small text</sup> and <sub>subscript</sub>.

---

## 15. Strikethrough

~~This text is crossed out~~

---

## 16. Mixed Content Example

### Shopping List
1. Apples — *fresh and organic*
2. Bananas — ~~out of stock~~
3. Coffee Beans — **Arabica**


> Pro Tip: Always check freshness dates.

---

**End of GFM Demo**
