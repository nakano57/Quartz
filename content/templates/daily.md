---
title: "<% tp.file.title %>"
created: <% tp.file.creation_date() %>
tags:
- post
- daily
---

<< [[<% fileDate = moment(tp.file.title, 'YYYY-MM-DD-dddd').subtract(1, 'd').format('YYYY-MM-DD-dddd') %>|Yesterday]] | [All Daily notes](/tags/daily) | [[<% fileDate = moment(tp.file.title, 'YYYY-MM-DD-dddd').add(1, 'd').format('YYYY-MM-DD-dddd') %>|Tomorrow]] >>

<% '?weather1%'.replace("?","%") %>

## 今日やること

<% tp.file.cursor() %>

## ふりかえり