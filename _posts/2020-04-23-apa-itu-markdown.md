---
title:  "Apa Itu Markdown"
header:
  teaser: "assets/images/apa-itu-markdown/teaser.jpg"
categories: 
  - Info
tags:
  - markdown
---


Markdown adalah sebuah tools untuk konversi text-to-HTML. Dengan Markdown, kita dapat menulis sebuah teks dengan mudah tanpa harus menghafal tag HTML. Markdown dibuat oleh [John Gruber](https://daringfireball.net/projects/markdown/) sejak tahun 2004 dan terus dikembangkan hingga sekarang.


Kelebihan menggunakan Markdown adalah format penulisanya yang simple sehingga kamu tidak akan butuh waktu lama untuk menghapalnya. Markdown translate dengan cepat ke bentuk HTML. Tidak ada closing tags yang hilang, tidak ada nested tags yang, tidak ada blok dibiarkan tanpa kontainer.

#### Markdown Format

```markdown
# Intro
Go ahead, play around with the editor! Be sure to check out **bold** and *italic* styling, or even [links](https://google.com). You can type the Markdown syntax, use the toolbar, or use shortcuts like `cmd-b` or `ctrl-b`.

## Lists
Unordered lists can be started using the toolbar or by typing `* `, `- `, or `+ `. Ordered lists can be started by typing `1. `.

#### Unordered
* Lists are a piece of cake
* They even auto continue as you type
* A double enter will end them
* Tabs and shift-tabs work too

#### Ordered
1. Numbered lists...
2. ...work too!

## What about images?
![Jefri Rendra Wiratmaja](https://lh3.googleusercontent.com/-wVyXpalMads/AAAAAAAAAAI/AAAAAAAAB88/u9T5SHmKZ6w/s640/photo.jpg)
```
#### HTML Format

```html
<h1>Intro</h1>
<p>Go ahead, play around with the editor! Be sure to check out <strong>bold</strong> and <em>italic</em> styling, or even <a href="https://google.com">links</a>. You can type the Markdown syntax, use the toolbar, or use shortcuts like <code>cmd-b</code> or <code>ctrl-b</code>.</p>
<h2>Lists</h2>
<p>Unordered lists can be started using the toolbar or by typing <code>*</code>, <code>-</code>, or <code>+</code>. Ordered lists can be started by typing <code>1.</code>.</p>
<h4>Unordered</h4>
<ul>
<li>Lists are a piece of cake</li>
<li>They even auto continue as you type</li>
<li>A double enter will end them</li>
<li>Tabs and shift-tabs work too</li>
</ul>
<h4>Ordered</h4>
<ol>
<li>Numbered lists...</li>
<li>...work too!</li>
</ol>
<h2>What about images?</h2>
<p><img src="https://lh3.googleusercontent.com/-wVyXpalMads/AAAAAAAAAAI/AAAAAAAAB88/u9T5SHmKZ6w/s640/photo.jpg" alt="Jefri Rendra Wiratmaja" />
```