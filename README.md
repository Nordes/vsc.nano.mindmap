# mindmap in vscode (vsc-nano-mindmap)
This extension support editing a mind map in a WYSIWYG inside VSCode.
![screenshots](https://season-studio.github.io/nano-mindmap/images/screenshots-vscode.gif)

## Features
- Show and edit mindmap
- Support xmind format
- Support multiple canvas in a mindmap file
- Support export to Markdown file (.md)
- Support import and export kittymind format (.km)
- Adaptive UI that change the locale from English to Simplified Chinese according to the enviroment of VSCode

## Installation
Install through VS Code extensions. Search for `vsc-nano-mindmap`

Visual Studio Code Market Place: `vsc-nano-mindmap`

## Usage
- Open any file with an extension **.xmind**, the UI will automatically show
- Edit the mind map by using the shortcuts in the toolbar or using the keyboard shortcuts (see below for the list)
- Create an empty file by executing VSCode command `new mind map`

## Commands
|Command|Feature|
|-------|-------|
|New Mind Map|Create an empty mind map file|
|Open Mind Map|Open a mind map file from File-Dialog with filter of extension name|

## Keyboard Shortcuts
|Key|Feature|
|---|-------|
|Ctrl+Alt+N|Create an empty mind map file|
|Ctrl+O|Open a mind map file|
|Ctrl+S|Save current mind map file|
|Ctrl+Z|Undo the last edit operation|
|Ctrl+Y|Redo the last operation you had undo|
|Tab|Add a new topic as a child of the focus topic|
|Enter|Add a new topic as a sibling of the focus topic|
|F3|Search a topic|
|F2|Edit the title of the focus topic|
|Delete|Remove the focus topic|
|Arrow Down|Goto the first children of the focus topic|
|Arrow Up|Goto the parent topic of the focus topic|
|Arrow Right|Goto the next sibling topic of the focus topic|
|Arrow Left|Goto the previous topic of the focus topic|

## Mouse Action
|Mouse Action|Feature|
|------------|-------------|
|Left button down in a topic and move the mouse| Dragging the topic to a new position|
|Left button down in canvas and move the mouse|Move the global canvas in the view|
|Wheel the middle button in canvas|Zoom the canvas|

## FAQ
- No support of the relationship line in the mind map at this time
- No support for rich-format text in notes of topic at this time
- We only support automatic layout mode, so you can NOT set location of topic in an absolute postion
- The operations "delete the current page" and "rename the current page" can NOT be revoked
- For saving memory, we clear all no-used attachments when you change the page. So all the edit operations you have done in the page can NOT be revoked once you change the page.
- The vscode extension SDK not support clearing undo&redo history without saving the document, but we will clear the history when you change the page(see the previous FAQ item). So we don't support invoking undo or redo action from the VSCode's menu. Instead, you can invoke this function using the extension's toolbar item or the shortcut of the keyboard

## Contact
Please report the issues on https://github.com/season-studio/vsc.nano.mindmap/issues

Or mail to season_studio@ooutlook.com if you have any question.
