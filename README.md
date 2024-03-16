## Obsidian Pandoc WPI Template
This is a template for the [Obsidian Enhancing Export](https://github.com/mokeyish/obsidian-enhancing-export/tree/main), a plugin for [Obsidian](https://obsidian.md/). It exports Obsidian markdown files to very professional Latex PDF files.

### Features
 - Support for all basic Obsidian markdown
 - Title Page and Footer set from front matter. Use `assignment`, `class`, `class_desc`, `author`, and `professor`.
 - H2 headings as sections/pages. Use asterick for unnumbered headings (ex. `## *Abstract` will be unnumbered and `## Introduction` will be numbered)
 - Code blocks with syntax highlighting
 - Inject raw latex with `latex` code blocks (allows for plots, `tikz` circuits, etc.)
	 - Some latex can also be written directly in with a code block (ex. `\lipsum[1]`)
 - Numbered and unnumbered equation blocks (default code blocks with \$\$ will be unnumbered and ones with `\being{equation}` will be numbered)
 
### Files
 - `wpi.lua` has formatting code unique for this template.
 - `wpi.tex` is the LaTeX template
 - `wpi.png` is used for the title page
 - `data.json` is the configuration for the Enhancing Export plugin
	 - `WPI` exports the markdown file to a PDF
	 - `WPI Latex` exports the markdown file to LaTeX (used for debugging purposes)

### Using
To use this template add the Enhancing Export plugin. Then, replace the `data.json` of the Enhancing Export plugin (`.obsidian\plugins\obsidian-enhancing-export`) with the one in this repository. Next copy `wpi.png` to your attachments folder. Finally place `wpi.lua` and `wpi.tex` into a folder of your choosing.
> You will most likely need to adjust the `data.json` file based on your particular vault file structure (mine is structured such that attachments are placed in `_Obsidan\Attachments` and Pandoc files are placed in `_Obsidan\Pandoc`).

### Credit
See credits in `wpi.tex`.
