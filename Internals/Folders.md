---
created: 2021-03-31
time: 05:46
tags:
---

# Folders - a misunderstood hero

# Search: folders, anti-folders
## Folders search
~~~
```query
path:Attachments
```
~~~
produces:
```query
path:Attachments
```


## Anti-Folders search
~~~
```query
path:-Attachments
```
~~~
produces:
```query
path:-Attachments
```

# Folder Note (plugin)
## Folder Brief
~~~
```ccard
type: folder_brief_live
```
~~~

# Folder Colors and Emojis (snippet)
[[CSS Development|CSS]] can help add colors and emoji for specific folder name or the folders starting with some string.^[[Adding Color to Obsidian--- A Rainbow of Possibility! - Feature requests - Obsidian Forum](https://forum.obsidian.md/t/adding-color-to-obsidian-a-rainbow-of-possibility/12805/11)]
![[Pasted image 20210418133355.png|right]]
#CSS
- Color for Folder that starts with a "03"
```css
    .nav-folder.mod-root>.nav-folder-children>.nav-folder>.nav-folder-title[data-path^="03"],
    .nav-folder.mod-root>.nav-folder-children>.nav-folder>.nav-folder-title[data-path^="03"] + .nav-folder-children{
    background-color: var(--Fold0);}
```
- Color for folder named “Daily Notes”
```css
    .nav-folder.mod-root>.nav-folder-children>.nav-folder>.nav-folder-title[data-path="Daily Notes"],
    .nav-folder.mod-root>.nav-folder-children>.nav-folder>.nav-folder-title[data-path="Daily Notes"] + .nav-folder-children{
    background-color: var(--Fold0);}
```
- Emoji for Folder that starts with a "03"
```css
.nav-folder.mod-root>.nav-folder-children>.nav-folder>.nav-folder-title[data-path^="03"] .nav-folder-title-content::before {
        content: '🌜';
        background-repeat: no-repeat;
        display: inline-block;
        width: 24px;
        height: 15px;
}
```