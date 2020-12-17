---
title: "Caferoman's Wiki"
keywords: wiki homepage
tags: [getting_started]
sidebar: wiki_sidebar
permalink: index.html
summary: This is personal wikipedia for about sing-a-song writer's note, reader's review and the things that I am interested in.
---

## About 조은찬(曺恩燦)

12월 2일에 태어난 조은찬의 관찰기록

[조은찬(曺恩燦)](about_cec)


## 三文章日記 (Write a diary with three sentences)

This is one of my To-Do-List in 2021.
The similar project was tried while I was in Sri-lanka(2005~2007) and this was much tough than the former.
(Keeping diarys every day in four languages: Korean, English, Sinhalese and German.)

[三文章日記(2020)](japanese_diary)

## Double D's Book Shelf - 더블디의 독서노트

독서노트라고 하기엔 너무 거창하지만 책을 읽으면서 마음에 들었던 구절과 짦은 소감이 포함된 페이지
곡을 쓰거나 대화를 하다가 가끔 읽었던 책의 특정 구절이 생각나지 않아 정리하기 시작한 페이지

[더블디의 독서노트](review_books)

{% include review_books.html %}

## Configure the sidebar

```bash
$ grep "찾을 문자열" * -rl | xargs sed -i 's/찾을 문자열/바꿀 문자열/g'
$ rename 's/mydoc/wiki/' *.md

```

## Generating PDF

If you want to generate PDF, you'll need a license for [Prince XML](http://www.princexml.com/). You will also need to [install Prince](http://www.princexml.com/doc/installing/).  You can generate PDFs by product (but not for every product on the site combined together into one massive PDF). Prince will work even without a license, but it will imprint a small Prince image on the first page, and you're supposed to buy the license to use it.

If you're on Windows, install [Git Bash client](https://git-for-windows.github.io/) rather than using the default Windows command prompt.

Open up the css/printstyles.css file and customize the email address (`youremail@domain.com`) that is listed there. This email address appears in the bottom left footer of the PDF output. You'll also need to create a PDF configuration file following the examples shown in the pdfconfigs folder, and also customize some build scripts following the same pattern shown in the root: pdf-discography.sh

See the section on [Generating PDFs][wiki_generating_pdfs] for more details about setting the theme up for this output.

## Blogs / News

For blog posts, create your markdown files in the \_posts folder following the sample formats. Post file names always begin with the date (YYYY-MM-DD-title).

The news/news.html file displays the posts, and the news_archive.html file shows a yearly history of posts. In documentation, you might use the news to highlight product features outside of your documentation, or to provide release notes and other updates.

See [Posts][wiki_posts] for more information.

## Markdown

This theme uses [kramdown markdown](http://kramdown.gettalong.org/). kramdown is similar to Github-flavored Markdown, except that when you have text that intercepts list items, the spacing of the intercepting text must align with the spacing of the first character after the space of a numbered list item. Basically, with your list item numbering, use two spaces after the dot in the number, like this:

```
1.  First item
2.  Second item
3.  Third item
```

When you want to insert paragraphs, notes, code snippets, or other matter in between the list items, use four spaces to indent. The four spaces will line up with the first letter of the list item (the <b>F</b>irst or <b>S</b>econd or <b>T</b>hird).

```
1.  First item

```
    alert("hello");
    ```

2.  Second item

    Some pig!

3.  Third item
```

See the topics under "Formatting" in the sidebar for more information.

## Automated links

If you want to use an automated system for managing links, see [Automated Links][wiki_hyperlinks.html#automatedlinks]. This approach automatically creates a list of Markdown references to simplify linking.

## Other instructions

The content here is just a getting started guide only. For other details in working with the theme, see the various sections in the sidebar.

{% include links.html %}

```