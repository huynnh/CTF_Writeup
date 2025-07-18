# Juice Shop Writeup: Score Board

## Challenge Overview
**Title**: Score Board  
**Category**: Miscellaneous  
**Difficulty**: ⭐ (1/6)  
**Goal**: Find the hidden scoreboard by locating the hidden URL of scoreboard page.

## Resolve

Step 1: When successfully accessing the Juice Shop website, press the **F12** key to open DevTool in Chrome.

Step 2: Navigate to **Sources** tab, then go to the **Pages** subsection. Look at *main.js* file.

Step 3: Press **Ctrl + F** in the main.js file to open searchbox and type the word "score". After a few tries to go through the result, there are a string might be the URL of scoreboard.

`"/score-board"`

Step 4: Try access localhost:3000/#/score-board. The scoreboard will be displayed.