# Description

The text used on the Firefox Add-ons listing.

## English

Vim Keys gives Firefox a Vim keyboard layer and keeps the 36 quick-site slots of Quick Sites.

Press f to label every link on screen with a short hint. Type the label to open it in the current tab, F to open it in a new active tab, or B to open it in a background tab that keeps the hints on screen, so you can queue several links in a row. Labels are at least two characters, and the characters you have already typed are dimmed so the rest of the label stands out.

o and t open a small panel for a typed URL (or a search). While you type it suggests matches from your saved slots, bookmarks, open tabs and browsing history, each row labelled with its source; Up/Down pick, Enter opens, Tab fills in the rest, and Ctrl+Enter opens in a background tab.

j/k/h/l, gg, G, d/e, Space, Backspace, 0, $ and 50% scroll the page the way they should, counts included. ;h/;l step through tabs and take a count (3;l skips three), g0/g$ jump to the ends, x closes and u restores. r reloads, , and . go back and forward. yy copies the page URL, yl the title, ;y a link URL from a hint, and V highlights the line under the cursor so y w can copy it. / finds in the page, * finds the word under the cursor, and n/N step through matches.

Every shortcut can be rebound in the settings page, in the toolbar popup, or in a JSON panel on the page itself (;e); the add-on refuses a keymap that conflicts with itself. ;p pauses everything on the current site and remembers it, for web apps with their own keyboard shortcuts. ? lists every binding, generated from the live keymap. Esc leaves a text field you are in, so a page that focuses its search box on load is usable immediately.

The quick-site slots are the whole of Quick Sites: m plus a slot key saves the current page, g o / g t / g b / g w plus a slot key opens it in the current tab, a new active tab, a background tab or a new window, and g l lists all 36. The list can be exported to and imported from a JSON file, and the five pickers can be renamed as one unit.

## 中文

Vim Keys 给 Firefox 加上了 Vim 风格的键盘层，并保留了 Quick Sites 的 36 个快捷站点槽位。

按 f 为页面上所有链接标上短提示，输入提示即可在当前标签打开；F 在新的活动标签打开；B 在后台标签打开并保留提示，可以连续打开多个链接。提示至少两个字符，已经输入的字符会变灰，剩下的字符更醒目。

o 和 t 打开输入面板，输入网址（或搜索词）。输入时会从已保存的槽位、书签、打开的标签和浏览历史里建议网址，每一行都标注来源；上下键选择，Enter 打开，Tab 补全，Ctrl+Enter 在后台标签打开。

j/k/h/l、gg、G、d/e、Space、Backspace、0、$、50% 按 Vim 的习惯滚动页面，支持数字前缀。;h/;l 切换标签并支持数字（3;l 往右跳三个），g0/g$ 跳到首尾，x 关闭，u 恢复。r 重新加载，, 和 . 前进后退。yy 复制当前网址，yl 复制标题，;y 复制提示所指链接的网址，V 高亮光标所在行、y w 复制它。/ 在页内查找，* 查找光标下的词，n/N 在匹配间跳转。

所有快捷键都能自定义：设置页、工具栏弹窗，或在页面上按 ;e 直接编辑 JSON；按键表自相冲突时扩展会拒绝保存。;p 可以在当前站点暂停全部快捷键并记住这个设置，适合自带键盘快捷键的网页应用。按 ? 可以查看由当前按键表实时生成的全部快捷键。Esc 会离开正在编辑的输入框，因此一打开就聚焦搜索框的页面也能直接使用。

快捷站点槽位保留了 Quick Sites 的全部功能：m 加槽位键保存页面，g o / g t / g b / g w 加槽位键分别在当前标签、新活动标签、后台标签、新窗口打开，g l 列出全部 36 个槽位。列表可以导出和导入 JSON 文件，五个前缀可以作为一个整体改名。
