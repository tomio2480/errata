---
layout: default
title: 一覧
---

# 技術系同人誌 正誤表

西原翔太（[@tomio2480](https://github.com/tomio2480)）が頒布した
技術系同人誌の正誤表を掲載しています．

{% if site.data.books and site.data.books.size > 0 %}
## 書籍一覧

<ul class="book-list">
{% for book in site.data.books %}
  <li>
    <a href="{{ '/books/' | append: book.slug | append: '/' | relative_url }}">{{ book.title }}</a>
    （正誤 {{ book.errata_count }} 件）
  </li>
{% endfor %}
</ul>
{% else %}
公開中の正誤表はまだありません．
{% endif %}

## 誤りを見つけたら

本の誤りを見つけた場合は，
[正誤報告フォーム](https://github.com/tomio2480/errata/issues/new/choose)
からお知らせください．内容を確認のうえ，正誤表へ反映します．
