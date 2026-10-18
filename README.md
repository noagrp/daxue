# 大学

A structured, reusable reader and explanation dataset for 《大学》.

## Content architecture

- `data/daxue.json` — source metadata, 经 / 传 structure, original text, explanations, vocabulary and思想小记
- `src/daxue-engine.js` — reusable group, navigation and full-text search engine
- `index.html` — reader UI only
- `manifest.webmanifest` / `sw.js` — PWA support

The JSON is intentionally independent from the website so other projects can reuse the material without parsing HTML.

## Base text

V1 follows 朱熹《四书章句集注·大学章句》, which arranges the text as 经一章、传十章.

Wikisource:
https://zh.wikisource.org/wiki/%E5%9B%9B%E6%9B%B8%E7%AB%A0%E5%8F%A5%E9%9B%86%E8%A8%BB/%E5%A4%A7%E5%AD%B8%E7%AB%A0%E5%8F%A5

Chinese Text Project:
https://ctext.org/si-shu-zhang-ju-ji-zhu/da-xue-zhang-ju1/zh

朱熹 states that the old text contained misplaced passages. His fifth transmission chapter also includes a reconstruction / supplement explaining 格物致知 because he regarded the original passage as lost. This project marks that supplement explicitly rather than presenting it as original 《礼记》 text.

## Editorial rule

The explanation first says what the passage means in its textual context. Textual variants, later interpretation, philosophical background and modern cautions belong in the note. Generic repeated statements should be avoided.

Original text is kept in Traditional Chinese. Explanations and notes are newly written in Simplified Chinese.
