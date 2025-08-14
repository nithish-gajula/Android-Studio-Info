# Android-Studio-Info

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
