# Reading View Enhancer

Reading View Enhancer is an Obsidian plugin that improves the reading experience in the reading view mode. It enhances reading view with several features to make it more convenient and comfortable.

## Features

### Overview

- **Block navigation with keyboard**
  - `ArrowDown` : select next "Block"
  - `ArrowUp` : select previous "Block"
- **Fold/Unfold with keyboard**
  - `ArrowLeft`/`ArrowRight` : Toggle fold/unfold
    - 📌 You can also fold/unfold collapsible callouts
- **Always on collapse indicators**
  - Make all the 'collapse indicators' visible
- **Prevent Table Overflowing**
  - Make tables scrollable to prevent table overflowing
- **Scrollable Code Block**
  - Make code blocks scrollable instead of line breaking

### Block Navigation with keyboard

> ⚡️ Settings > Reading View Enhancer > Enable Block Selector

https://user-images.githubusercontent.com/78684419/228733812-26bfa11a-f246-4153-83ea-eed9aae39753.mov

You can select blocks in the reading view by clicking on them.
When you select a block, it will be highlighted,
and you can navigate between blocks using the arrow keys.

If the selected block is too long, the plugin will automatically
scroll to see the block's top or bottom, loading adjacent blocks
that are not in the DOM tree yet.

- `ArrowDown` : select next "Block"
- `ArrowUp` : select previous "Block"
- `ArrowLeft`/`ArrowRight` : toggles fold/unfold

❗️ This feature only works on desktop.  
✨ This feature is inspired by Notion's block navigation.

#### What is "Block"?

In this plugin, a "block" refers to an HTML element that can be
considered a distinct unit of content within a markdown document.

Such as paragraphs, headings, lists, tables, code blocks, quotes,
media elements, and callouts are blocks.

#### Block Color

> ⚡️ Settings > Reading View Enhancer > Block Color

You can set a color for the block highlight effect.

### Always On Collapse Indicators

> ⚡️ Settings > Reading View Enhancer > Always on collapse indicator

By default, collapse indicators are invisible until it gets hovered.

<img width="400" alt="no-indicator" src="https://user-images.githubusercontent.com/78684419/228733972-6b364496-071b-469a-a401-656b3df27311.png">

Using this option,

<img width="400" alt="turn-on-indicator" src="https://user-images.githubusercontent.com/78684419/228734050-54d19f73-35cd-4eba-ae33-8d91f7bed180.png">

you can make indicators always visible.

<img width="400" alt="has-indicator" src="https://user-images.githubusercontent.com/78684419/228734081-99e58a5d-b6b2-4418-92f1-b47db403e7ae.png">

### Prevent Table Overflowing

> ⚡️ Settings > Reading View Enhancer > Prevent Table Overflowing

https://user-images.githubusercontent.com/78684419/228734185-aca9e6ee-711e-4929-8e10-a269a43b97f8.mov

You can make tables horizontally scrollable to prevent table overflowing.

In Obsidian v1.1.16, table with a long text makes a horizontal scroll bar on the whole view,
which makes it inconvenient in a mobile environment.

### Scrollable Code

> ⚡️ Settings > Reading View Enhancer > Scrollable Code

By default, codes are placed in new line when it's too long.

<img width="400" alt="before-code-scroll" src="https://user-images.githubusercontent.com/78684419/228734385-2cf4650a-0559-48c8-a1ad-3229f68b40a1.png">

With this option,

<img width="400" alt="turn-on-code-scroll" src="https://user-images.githubusercontent.com/78684419/228734481-5ed5994c-ca63-4777-9341-8da105afcc94.png">

You can make code blocks scrollable instead of line break.

<img width="400" alt="code-scroll" src="https://user-images.githubusercontent.com/78684419/228734516-77f5446f-2669-43d5-8428-65e400e7a00d.png">

## How to install manually?

There might be various ways to install this plugin.

After installation,

1. Go to `Settings > Community Plugins > Installed plugins`
2. Refresh the list
3. Turn on the switch of "Reading View Enhancer" to enable the plugin

### Using Obsidian42-BRAT (Recommended)

By using [Obsidian42-BRAT](https://obsidian.md/plugins?id=obsidian42-brat), you could easily install & update this plugin.

1. Install **Obsidian42-BRAT**
2. Enable Obsidian42-BRAT
3. Go to Obsidian42-BRAT options page
4. Beta plugins list > `Add Beta plugin`
5. Paste this `https://github.com/Galacsh/obsidian-reading-view-enhancer`
6. After installation is done, go to `Settings > Community Plugins > Installed plugins`
7. Refresh the list
8. Turn on the switch of "Reading View Enhancer" to enable the plugin

### Using `curl`

Before to run the code, make sure to change `[VAULT]` and `[RELEASE_VERSION]` into a real value.

```shell
# Go to your vault's plugins folder
cd [VAULT]/.obsidian/plugins
# Make a directory
mkdir obsidian-reading-view-enhancer
cd obsidian-reading-view-enhancer
# Download
curl -OL https://github.com/Galacsh/obsidian-reading-view-enhancer/releases/download/[RELEASE_VERSION]/main.js
curl -OL https://github.com/Galacsh/obsidian-reading-view-enhancer/releases/download/[RELEASE_VERSION]/styles.css
curl -OL https://github.com/Galacsh/obsidian-reading-view-enhancer/releases/download/[RELEASE_VERSION]/manifest.json
```

### By downloading manually

1. Download this files from the latest [release](https://github.com/Galacsh/obsidian-reading-view-enhancer/releases)
   - `main.js`
   - `styles.css`
   - `manifest.json`
2. Create a directory(`obsidian-reading-view-enhancer`) inside `.obsidian/plugins`
3. Move files to your vault's `.obsidian/plugins/obsidian-reading-view-enhancer` folder
