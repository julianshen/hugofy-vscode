# Change Log

All notable changes to the "hugofy" extension will be documented in this file.

Check [Keep a Changelog](http://keepachangelog.com/) for recommendations on how to structure this file.

## 0.3.4

- refactor: prefetch theme list: only work on a hugo project
- refactor: new post prompt: default filename to empty. slug: only process latin1

## 0.3.3

- fix: fixup default keybindings

## 0.3.2

- refactor: add default keybindings, show message on success build

## 0.3.1

- refactor: change theme config key to `hugo.defaultTheme` since `launch.json` is general
- fix: fix extension recommendations

## 0.3.0

- fix: theme dir for `xxx-theme` or `theme-xxx`
- fix: do not check theme exists on non-hugo site directory

## 0.2.9

- fix: newPost: show detailed error message
- fix: set correct theme name from config on extension activation
- fix: check theme exists, if not, notify the user to "Set Theme"

## 0.2.8

- fix: fixup path problem under Windows

## 0.2.7

- refactor: add actions when theme download failed or succeed

## 0.2.6

- refactor: optimized download theme feature

## 0.2.5

- fix: Windows path separator

## 0.2.4

- refactor: check hugo in PATH or not, if not notify the user
- fix: show detailed build error

## 0.2.3

- refactor: show hugo server start error details

## 0.2.2

- refactor: optimized set theme and download theme feature

## 0.2.1

- refactor: open local hugo blog: prevent browser cache problem

## 0.2.0

- fix: check theme set or not before newPost(), show detailed error on new site error

## 0.1.9

- docs: update README.md

## 0.1.8

- fix: fixup set theme

## 0.1.7

- fix: fixup theme download

## 0.1.6

- refactor: refine console log
- docs: update development document

## 0.1.5

- use [transliteration](https://www.npmjs.com/package/transliteration) instead of limax
  which cause problem under webpack and has too many dependencies

- use webpack to [bundle the extension](https://code.visualstudio.com/api/working-with-extensions/bundling-extension),
  thanks [this PR](https://github.com/Microsoft/vscode-references-view/pull/50)

## 0.1.4

- chore: fixup getThemesList.ts line ending (CRLF to LF)
- docs: updated CHANGELOG.md and README.md

## 0.1.3

- chore: extension logo added

## 0.1.2

- docs: updated CHANGELOG.md and README.md

## 0.1.1

- refactor: lint the code, more friendly error message
- fix: do not start the server again if already started
- feat: add `New Post` action on current folder right click event
- feat: support normalize path name to **slug** friendly path

  Currently supports, but not limited to, the following scripts:

  - **Latin**: e.g. English, français, Deutsch, español, português

  - **Cyrillic**: e.g. Русский язык, български език, українська мова

  - **Chinese**: e.g. 中文 (converts to Latin script using Pinyin with optional tone number)

  - **Japanese**: e.g. ひらがな, カタカナ (converts to Romaji using Hepburn)

  For example:

  Cyrillic: `Я люблю русский/index.md`  => `ya-lyublyu-russkij/index.md`

    Chinese: `你好/index.md` => `ni-hao/index.md`

    Japanese Romaji: `私は ひらがな が大好き/index.md` => `ha-hiragana-gaki/index.md`

## 0.1.0

[Fix] Fixed start server error

## 0.0.2

- [Fix] Server Stop workd on windows

## 0.0.1

- Initial release