---
title: "The 1st Note Here"
date: 2025-03-29T10:42:45Z
draft: false
description: ""
---

## Taxonomy

* categories = {"bundle", "unit", "digest", ...}
* sources = 语料/主题的来源
* tags = {"単語", "文法", ...}


## Cheat Sheet 

使用 UTC 时区新建文章：

```sh
TZ=UTC hugo new content <path to the target>
```

本地预览：（不丢失样式）

```sh
hugo server --baseURL="http://localhost:1313/"
```

振假名：
これは<ruby>日<rt>に</rt>本<rt>ほん</rt>語<rt>ご</rt></ruby>です。

振假名（html 代码）：

```html
これは<ruby>日<rt>に</rt>本<rt>ほん</rt>語<rt>ご</rt></ruby>です。
```

## Prompt Magic

辨析/對比：

```text
你是一位有著豐富的日語教學經驗的專家。

我將給出一些
{
我認為容易混亂的單字或者短語用法。
}
你將為他們寫出對比/辨析的說明，並且都有簡單的例句。

你的所有輸出都在代碼塊中，以便我檢查格式和粘貼到我的筆記本上。

輸出時，你嚴格遵循並利用markdown格式。

- 你輸出的內容起一個標題，作為h2
- 如果你的h2帶括弧讀音，則在h2中改為html的ruby標籤來標註振假名
- 你有這樣的h3:{詞語解釋、例句對比、注意點}
- 請不要在文本中使用任何黑體和斜體樣式；如果我與vscode協作，則格式吻合當前文檔即可
- 在輸出的代碼塊內，h2底下的第一行是（ChatGPT生成）。

你給出的解釋是中文，你的例句有日文與參考翻譯。

如果我與vscode協作，則直接追加到當前文件的最底下，並且禁止刪除當前存在的文段。

如果你明白了我的指令，請告訴我你明白了。
```
