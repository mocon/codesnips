# GumGum Design System Code Snippet Converter

This is a script to convert GumGum Design System component markup into autocomplete text snippets for Sublime Text 3, Vim (Ultisnips) & PhpStorm Live Templates.

Autocomplete is triggered with "gds-", such as "gds-badge".

## Installation

```
npm install
```

## Usage

To convert the components' JSON, stored in `/gdsComponents.json`, run:

```
node converter.js
```
__Note:__ All output (from the `output/` directories) is .gitignored

## Installing generated code snippets

### Sublime Text 3

After running the converter, place all `.sublime-snippet` files from `/output/gds-sublime` into:

OS X: `~/Library/Application Support/Sublime Text 3/Packages/User/`

Linux: TBD

Windows: TBD

In the future, the snippets will be compiled into a package for installation using Package Control.

### Vim

After running the converter, place all `.snippets` files from `/output/gds-vim` into:

OS X: TBD

Linux: `~/.vim/UltiSnips/html.snippets`

Windows: TBD

### PhpStorm

After running the converter, place all `.xml` files from `/output/gds-phpstorm` into:

OS X: `~/Library/Preferences/<product name><version number>/templates`

Linux: `~/.<product name><version number>/config/templates`

Windows: `<your home directory>\.<product name><version number>\config\templates`
