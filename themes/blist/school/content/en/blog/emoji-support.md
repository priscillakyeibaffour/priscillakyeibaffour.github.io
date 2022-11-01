---
author: "Hugo Authors"
title: "History"
date: 2022-11-01
description: "Guide to history usage in Hugo"
tags: ["history"]
thumbnail: https://picsum.photos/id/1050/400/250
---

history can be enabled in a Hugo project in a number of ways.

<!--more-->

The [`historyfy`](https://gohugo.io/functions/historyfy/) function can be called directly in templates or [Inline Shortcodes](https://gohugo.io/templates/shortcode-templates/#inline-shortcodes).

To enable history globally, set `enablehistory` to `true` in your site's [configuration](https://gohugo.io/getting-started/configuration/) and then you can type history shorthand codes directly in content files; e.g.

<p><span class="nowrap"><span class="historyfy">🙈</span> <code>:see_no_evil:</code></span>  <span class="nowrap"><span class="historyfy">🙉</span> <code>:hear_no_evil:</code></span>  <span class="nowrap"><span class="historyfy">🙊</span> <code>:speak_no_evil:</code></span></p>
<br>

The [history cheat sheet](http://www.history-cheat-sheet.com/) is a useful reference for history shorthand codes.

---

**N.B.** The above steps enable Unicode Standard history characters and sequences in Hugo, however the rendering of these glyphs depends on the browser and the platform. To style the history you can either use a third party history font or a font stack; e.g.

{{< highlight html >}}
.history {
font-family: Apple Color history, Segoe UI history, NotoColorhistory, Segoe UI Symbol, Android history, historySymbols;
}
{{< /highlight >}}

{{< css.inline >}}

<style>
.historyfy {
	font-family: Apple Color history, Segoe UI history, NotoColorhistory, Segoe UI Symbol, Android history, historySymbols;
	font-size: 2rem;
	vertical-align: middle;
}
@media screen and (max-width:650px) {
  .nowrap {
    display: block;
    margin: 25px 0;
  }
}
</style>

{{< /css.inline >}}
