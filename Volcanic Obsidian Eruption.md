---
created: 2021-03-29
summary: "A guide to the Obsidian.md ecosystem, from @riddyrayes"
version: 0.3
cssclass: logmode
---

# Stages in Eruption
A local wiki style introduction to **Obsidian ecosystem** with a 🌋 volcano theme^[The names of major levels inspired from the TL;DR of the article https://sciencing.com/stages-volcano-eruption-8549867.html]

- [[#The Quakes]] - the very basics for starting hour
- [[#The Emissions]] - the important information for starting week
- [[#The Venting]] - Knowledge Management Techniques, Integration with other Editors, Folders and Tags best uses
- [[#The Buildup]] - technical aspects of note taking and managing - Diagrams, Equations
- [[#The Collapse]] - applied aspects of note making and managing - Task Management, Zotero Integration and Citation management
- [[#The Explosion]] - spider webbing a large vault
- [[#The Growth and failures]] - growing into a galactic civilization
- [[#The Ash and Lava]] - sharing the vault to public 
- [[#Back to Dormant]] - further development in ecosystem and workflow

> 🛑 DON'T PANIC

```ad-info
- Reader is requested to only read ==The Quakes== part on day 1 of using Obsidian.
- Reader may use CTRL+Scroll to increase or decrease the font size of the text.
```
---
<br>
<br>


# The Quakes
```abstract
the very first of the first stuff
``` 

```ad-tip
title: The reader is advised to 
- Open a blank vault and make a note
- readout the Official Help pages alongside this section of the wiki; available at bottom left '?' button.
```
1. Create a blank note.
2. Writing note on Obsidian uses two modes, Preview and Edit. It can be toggled from top right button.
![[Pasted image 20210413154347.png]]

The first Hotkeys to learn:
- CTRL+E - Switch from **Preview** to **edit mode**
- CTRL+P - Open **command palette**, to search for various operations to do
- CTRL+O - Quickly open some note or create a new one

<br>

- *Obsidian* is a file editor and databasing tool, wrapped around as a note writing and note taking tool, with an ambition to become a "second brain".
- It is very customizable and programmable in its functionality and appearance.
- Every knowledge of file and folders works on Obsidian vaults.
- The learning curve is NOT steep, but the learning and setup time requires a little patience.
- For readers information, Obsidian is built on [Electron](https://www.electronjs.org/)

## Markdown Syntax _(unofficially) Obsidian flavored_

Writing in Obsidian uses basic Markdown syntax. 
### Links and Embeds
`[[note]]`
`![[note]]`
`[[note#heading]]`
`![[pic.png]]`
`[[file.extension]]`

### Text Styles
`**bold**`
`*italic*` `_italic_`
`~~strikethrough~~`
`> quotes`

### Headings

~~~
# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5
###### Heading 6
~~~


## Necessary Settings
![[Pasted image 20210413140132.png|right|150]] CTRL+, or click on Settings icon at bottom right to open settings.
There would be a list of OPTIONS to open from:

The default settings works fine mostly, the things that advised to change and to be informed about are:

### Editor
- **Spell Check** - Currently only Available for American English
- **Readable Line length** - Turning it off makes the editor take use of total available width to type in
- **Fold** - Fold headers and lists using a little triangle, folding is not lost after a note is closed
- **Default *New Pane* mode** - Open in Edit mode or in Preview mode as default
- **Auto convert HTML** - While copying from any website it converts the pasted text to a preview friendly version. Pasting using CTRL+SHIFT+V pastes the raw text. Although this would be frustrating for pasting codes as it converts `[` to `\[`

```ad-warning
Do not turn on Vim key bindings if you are unfamiliar with Vim editor.
```
### Files & Links
- **File deletion**
![[Pasted image 20210413143412.png|500]]
- **Default location** - *Same folder as current file* is a desirable option if reader plans to use [[#Folders|folders]] in the vault
- **Detect all file extensions** - Detects all available files and when clicked, opens in default app.
### Appearance
1. Click on Browse: ![[Pasted image 20210413152628.png|400]]
2. Choose a theme. New users are advised to try "Obsidinite" theme for first use.
3. Click on Use
### Hotkeys
Choose a "Hotkey" configuration for the commands

### About
- Keep Automatic updates turned on
- Make sure to reinstall Obsidian of the installer version becomes too old
- Turn on Receive insider builds if user is on [[Obsidian Catalyst]]

### Account
- No account required if Obsidian Sync, Publish or Receive insider builds are not desired

### Core plugins
Most plugins appear in the little left menu. ![[Pasted image 20210413142730.png|right|30]] They have a separate settings options list:
![[Pasted image 20210413150810.png|150]] ^46dd
1. [[#Tags]] - Use `#tags` to group notes based on any label. The tag pane arrives at the right pane. Drag to any preferable spot.
2. **Page Preview** - Hover over links to preview note.
![[Pasted image 20210413150446.png|500]]
3. **Starred** - Make a list of notes that are "Starred"
4. **Markdown format importer** - Turn off if reader is not a Roam or Bear user
5. [[#Daily notes]]
6. [[#Templates]]
7. **Zettelkasten prefixer** - For Zettelkasten user can be used an 'Inbox' of notes
8. **Random note** - Opens a random note
9. **Outline** - Open a "ouline" from all `#` headers from Note options at top right triple dots.
 ![[Pasted image 20210413152947.png]] ![[Pasted image 20210413153143.png]] ![[Pasted image 20210413151412.png|200]]
10. **Slides** - Use a note to start a full screen presentation
11. **Audio recorder** - Record audio
12. **Workspace** - Save the current configuration of notes as "Workspace"
![[Pasted image 20210413151525.png|200]]
13. **File recovery** - File versioning and recovery for notes
14. **Publish and Sync** - Paid [[Obsidian.md]] features

# The Emissions
> *the important information for beginners*
## In-built features
> More in the article [[Internals]]

## Mobile-Desktop interaction
The use of mobile app and desktop apps different in a lot ways. There are some best practices to find the best out of the synchronization.

## Sync and Backup
### Obsidian Sync
> More in the article [[Obsidian.md#Sync]]

### GitHub repo Sync
> More in the article [[GitHub#GitHub repo Sync]]

### Drive Backup and Sync
Services like Google Drive, OneDrive and iCloud
### Devices Sync
- [[SyncThing]] - an open-source solution to sync in most devices with a ~10 second lag from Obsidian Mobile

## Templates
> More in the article [[Templates]]
## Daily Notes
> More in the article [[Daily Notes]]
### Periodic Notes
## The Community ❤️
## Community Plugins
> More in article [[Community Plugins]]

### Calendar Plugin

### Sliding Panes Plugin
## CSS Themes and Snippets
> More in article [[Community Themes]]
There are community themes that can be downloaded from settings.

### Exploring Snippets
> More in article [[CSS Snippets]]

There are numerous CSS snippets from the community used for various purposes.
### Development
> More in the article [[CSS Development]]

# The Venting
> _Knowledge Management Techniques, Other Editors, Folders, Tags_
## Knowledge Management, Linking and Styling of Notes
> More in the article [[Mechanisms]]

^[https://forum.obsidian.md/t/cataloging-classification-information-science-pkms-and-you/10071]

## Markdown Manipulation and more
- [[Zettlr]]
- [[Pandora]]
- [[VScode]]
- [[Typora]]
- [[LogSeq]]

## Folders
> More in article [[Folders]]

^[https://forum.obsidian.md/t/increasingly-atomic-folders-a-workflow/14345/1]

## Tags
> More in article [[Tags]]

## Other Applications
- [[Xjournal++]]

## External Embeds
> More in the article [[External Embeds]]
- Calendar
- Live Weather


# The Buildup
> _technical aspects of note taking and managing_
## Search

## Query and Dataview
> More in the article [[Query and Dataview]]

## Diagrams
> More in the article [[Mermaid Diagrams]]

## Equations
> More in the article [[MathJax Equations]]
> For further rigorous mathematics, refer to [[LaTex]] integration

## Handling Images
> More in the article [[Images]]

## Surfing the Web
- [[Raindrop]]
- [[Markdownload]]
- [[Tab copy]]

## Mail
> More in article [[Mail#From mail to note]]

## Videos
> More in the article [[Videos]]

## Podcasts

# The Collapse
> _applied aspects of note making and managing_
## Zotero Integration
> More in article [[Zotero]]
## Active Recall and Spaced Repetition
> More in article [[Mechanisms#Active Recall and Spaced Repetition]]
- [[Anki]]
- [[RemNote]]
- [[Neuracache]]

## Task Management
> More in article [[Mechanisms#Task Management]]
- GTD Plugin
- Kanban Boards
- Day planner


# The Explosion
> _spider webbing a large vault_
## The Graph View
> More in the article [[Graph View]]
### Local Graph


## Idea Emergence
# The Growth and failures
> _growing into a galactic civilization_
## File recovery
## 

# The Ash and Lava
> *sharing the vault to public*
## Obsidian Publish
> More in the article [[Obsidian.md#Publish]]
## GitHub Pages
## Tweets
## Mail
> More in article [[Mail#From note to mail]]


# Back to Dormant
> _further development in ecosystem and workflow_
## LaTex
> More in the article [[LaTex]]

For more rigorous use of mathematical notation and equations, chemical structures and equations, diagrams, we must use the industry standard - [[LaTex]]. Various Tex utility software like TexStudio, services, or even Vim can be used to create LaTex documents but for the purpose of keeping a familiar aspect to a unfamiliar wold, we shall use [[VScode]] to write LaTex documents and integrate with Obsidian.

## LYT Kit
The kit suggests readers to have at least 100 notes. This is a best place to expand more on [[Mechanisms]].


# References