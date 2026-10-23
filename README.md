# Vim Keys

Vim-style keyboard control of Firefox: follow links with hints, open URLs,
scroll, switch tabs, and keep the 36 quick-site slots of Quick Sites.

In memory of Vimperator.

## Install

[**Vim Keys on addons.mozilla.org**](https://addons.mozilla.org/en-US/firefox/addon/vimkeys/)

Firefox 140+ (Android 142+). Install it and press `?` for the key list — no
setup, no account.

## Screenshots

![Press f: every link gets a short hint label. Type it to open the link, F for a new tab, B for a background tab that keeps the hints on screen.](Screenshots/01-hints.png)
![Press ?: every shortcut, generated from the live keymap, grouped by what it does.](Screenshots/02-help.png)
![Press ;e to edit every setting, including the keymap, in a panel on the page.](Screenshots/03-settings.png)
![All 36 quick-site slots in the settings: a URL and a title each, with Open, New tab and Clear, and the list can be exported and imported as JSON.](Screenshots/04-slots.png)

## What it does

Vim Keys gives Firefox a Vim keyboard layer and keeps the 36 quick-site slots of Quick Sites.

Press f to label every link on screen with a short hint. Type the label to open it in the current tab, F to open it in a new active tab, or B to open it in a background tab that keeps the hints on screen, so you can queue several links in a row. Labels are at least two characters, and the characters you have already typed are dimmed so the rest of the label stands out.

o and t open a small panel for a typed URL (or a search). While you type it suggests matches from your saved slots, bookmarks, open tabs and browsing history, each row labelled with its source; Up/Down pick, Enter opens, Tab fills in the rest, and Ctrl+Enter opens in a background tab.

j/k/h/l, gg, G, d/e, Space, Backspace, 0, $ and 50% scroll the page the way they should, counts included. ;h/;l step through tabs and take a count (3;l skips three), g0/g$ jump to the ends, x closes and u restores. r reloads, , and . go back and forward. yy copies the page URL, yl the title, ;y a link URL from a hint, and V highlights the line under the cursor so y w can copy it. / finds in the page, * finds the word under the cursor, and n/N step through matches.

Every shortcut can be rebound in the settings page, in the toolbar popup, or in a JSON panel on the page itself (;e); the add-on refuses a keymap that conflicts with itself. ;p pauses everything on the current site and remembers it, for web apps with their own keyboard shortcuts. ? lists every binding, generated from the live keymap. Esc leaves a text field you are in, so a page that focuses its search box on load is usable immediately.

The quick-site slots are the whole of Quick Sites: m plus a slot key saves the current page, g o / g t / g b / g w plus a slot key opens it in the current tab, a new active tab, a background tab or a new window, and g l lists all 36. The list can be exported to and imported from a JSON file, and the five pickers can be renamed as one unit.

## Keys

| Keys | What it does |
| --- | --- |
| `f` / `F` / `B` | Label the links: open in this tab, a new active tab, or a background tab that keeps the hints on screen |
| `o` / `t` / `b` | Type a URL or a search, with suggestions from slots, bookmarks, tabs and history, in this / a new / a background tab |
| `j` `k` `h` `l` `gg` `G` `d` `e` `<Space>` `<Backspace>` `0` `$` `%` | Scroll, with Vim counts (`3j`, `50%`) |
| `;h` / `;l` | Step through tabs, with a count (`3;l`) |
| `g0` / `g$` / `x` / `u` | First / last tab, close, restore |
| `yy` / `yl` / `;y` | Copy the page URL, the title, or a link URL from a hint |
| `V` then `y w` | Highlight the line under the cursor and copy it |
| `/` `*` `n` `N` | Find in the page, find the word under the cursor, next / previous match |
| `?` | Every shortcut, generated from the live keymap |
| `;e` | Edit the settings, including every key binding, in a panel on the page |
| `;p` | Pause Vim Keys on the current site, and remember it |
| `m` + key | Save the current page into one of the 36 quick-site slots |
| `g o` / `g t` / `g b` / `g w` + key | Open a slot in this tab, a new tab, a background tab, or a new window |
| `g l` | The list of saved slots |

Every shortcut can be rebound, and a keymap that conflicts with itself is
refused. A count works wherever it makes sense: `10j`, `3<Space>`, `5%`, `3;l`.

Press `?` in any page for the complete, always-current list.

## One browser restriction

Firefox does not let any extension run a content script on `addons.mozilla.org`
(including this add-on's own page), `accounts.firefox.com`,
`support.mozilla.org` and a few other Mozilla sites, or on privileged pages such
as `about:addons`, `about:debugging`, `view-source:` and the PDF viewer. Vim
Keys is silent there; this is a browser security rule that no extension can
override. After installing from AMO, open any normal page to use it.

## Links

- Add-on: https://addons.mozilla.org/en-US/firefox/addon/vimkeys/
- Issues: https://github.com/lylehust/Vim-Keys/issues
