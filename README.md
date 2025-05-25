# dotfiles / new computer setup

this is my general suite of tools and settings to quickly get a new machine in a comfortable working state

- download & install:
  - [brave browser](https://brave.com/download/) 
    - set as default browser
    - duckduckgo as default search
  - [iterm2](https://iterm2.com/)
  - [sublime text](https://www.sublimetext.com/)
  - [oh my zsh](https://ohmyz.sh/)
  - [vs code](https://code.visualstudio.com/)
  - [rectangle app](https://rectangleapp.com/)
  - [powerline fonts](https://github.com/powerline/fonts) (also [Fira Code](https://github.com/tonsky/FiraCode) for IDE use if desired)
  - [nvm](https://github.com/nvm-sh/nvm)
    - `nvm ls-remote` to see available versions
    - `nvm install 22` to install node 22
  - [docker](https://www.docker.com/)

- [generate new ssh key](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent#generating-a-new-ssh-key) & add to github profile

- update iterm2 settings:
  -  Profiles > Colors > Solarized Dark
  -  Profile > Text
      - Blinking vertical bar
      - Use built-in Powerline glyphs
      - Font: Meslo LG L for Powerline, size 14

- update VS Code 
  - add extensions: Prettier, eslint, Python, Svelte, Docker, etc.
  - settings.json:
```
  {
      "workbench.colorTheme": "Solarized Dark",
      "telemetry.feedback.enabled": false,
      "telemetry.telemetryLevel": "off",
      "files.autoSave": "onFocusChange",
      "workbench.editor.wrapTabs": true,
      "workbench.commandPalette.experimental.enableNaturalLanguageSearch": false,
      "workbench.enableExperiments": false,
      "editor.fontFamily": "Fira Code",
      "editor.fontLigatures": true
  }
```

- copy this repo's .zprofile and .zshrc to your home directory:
  - `cp .zprofile ~/.zprofile`
  - `cp .zshrc ~/.zshrc`

- run `source ~/.zshrc`