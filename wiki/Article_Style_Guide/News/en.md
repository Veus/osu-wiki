# News

News articles exist on a slightly different system to the main osu!wiki, but follow similar principles. Writing them involves careful attention to a few key features and formats as outlined below.

As always, all news articles should aim to have proper spelling and grammar at a bare minimum, as well as having correct and up-to-date information.

## Repository directory

The following standards apply only to articles written for the news, and saved in the `news/` directory.

## Locales

The news system does not support locales at this time. All articles must be in British English, with a consistent register. 

What this register entails depends on the focus and tone of your article, but it must be consistent. Articles that sound professional must always sound professional. Articles that are conversational must be always conversational.

## Writing standards

All news articles must be written with a few key concepts in mind - conciseness, audience, and presentation.

### Conciseness

News articles should be short and sweet, with appropriate information condensed as much as possible without being overly dense. 

Provide links to in-depth resources instead of referencing them directly in-text. Use visual displays wherever possible to convey large amounts of information at a glance.

### Audience

_osu!_'s chief audience is mainly teenagers and young adults, though we are an all-ages community. Consider the attention span of said demographic - conciseness ties in very closely to this.

Consider well what you write within your article and whether it would interest the community at large enough to warrant including it.

### Presentation

News articles must aim to be as pleasingly neutral as possible in terms of presentation. 

Pleasingly neutral, however vague, refers to an article that is both light and robust, saying what it needs to say without giant blocks of text. It must be consistent in formatting, style and register. Large quantities of information should be supported or supplanted with visual aids.

## Formatting

### Article filenames

News articles are markdown files (``.md``) are named under the following format:

``yyyy-mm-dd-<article title>.md``

Where ``yyyy`` is year as 4 digits, ``mm`` is month as 2 digits, and ``dd`` is the date as 2 digits.

Article title strings for file names are the title of the article itself with all spaces replaced with hyphens (`-`), and all additional characters such as periods (`.`), exclamation marks (`!`), question marks (`?`) and commas (`'`) removed with no replacement.

### File headers

All news article files must include a basic header which includes information about the article's title and published date. This must follow the format below:

```
---
layout: post
title: "Aspire 2017 Stage Two: osu!taiko Concludes"
date: 2017-08-17 03:00:00 +0000
---
```

``layout`` must alway be set to ``post``.

``title`` must represent the article's full title and name, complete with any appropriate formatting. Markdown formatting is disallowed in this string.

``date`` must represent a combined string displaying a calendar date in ISO 8601 format (2017-08-17), followed by a 24 hour time string (03:00:00), followed by a time offset from UTC (+0000). This date is used to determine the "xx minutes/hours/days ago" display on the website when referring to the publish dates of visible news articles.

### Markdown

The wiki uses a partial implementation of GFM (GitHub Flavored Markdown) with the following exceptions:

#### Titles

News articles do not use traditional Markdown titles in any capacity whatsoever.

#### Headers

Headers are currently limited to header level 2 (``##``) at the current time.

#### Bold

Bolding is reserved for highlighting objects or phrases of importance, be them players, scoring, or whatever else is contextually considered a focus of the article in question.

#### Italics

Italics is used uncommonly to accent phrases or statements of interest within the conversational register. It may also be used to designate names of other creative works, such as the _osu! Coffee Hour_ or the _Aspire Beatmapping Contests_.

#### Horizontal bar

Horizontal bars must be used sparingly and only in situations where content needs to be cleanly and definitively separated from the rest of the article.

#### Tables

We do not recommend using Markdown tables for displaying data in news articles. Visualising the data using an image is likely to be more pleasing and more accessible to most users.

### Images

#### Repository directory

All images linked to news articles must either be hosted on osu! servers (ie: assets.ppy.sh) or placed within and referenced from the wiki shared image repository.

News articles that use images have their own folder within ``/wiki/shared/news/`` using the same naming format as their filename, with the exception of the ``.md`` suffix.

Example:

``/wiki/shared/news/2017-08-17-news-article-standards/banner.jpg``

#### Formats and quality

Images used in news articles must be in JPG format at quality 9 (90) to quality 10 (100). PNG use is acceptable in instances where the filesize is small, or quality cannot afford to be compromised.

#### Filesize

All images must be optimized as much as possible. We recommend the use of [FileOptimizer](http://nikkhokkho.sourceforge.net/static.php?page=FileOptimizer) to do this quickly and consistently.

#### Captions

Images are not soft-captioned using Markdown except in stylistic circumstances. They may be hard-captioned where contextually appropriate.

### HTML and embedded content

Limited HTML use for the purposes of embedding off-site content such as YouTube videos, Twitch VODs or other applets designed to showcase osu! or osu! related content is allowed.

``<center>`` tag use (or any equivalent styling such as ``<p align='center'>``is disallowed due to the news system styling automatically centering non-text elements.

The width of all embedded content frames must be set to ``width: 100%``. To be included in articles in general, embedded content must support display at full-width styling without breaking or looking awful.

### Linking to osu! related information

All osu! related information should aim to use the new site wherever possible.

This includes forum threads (``https://osu.ppy.sh/community/forums/13``), user profiles (``https://osu.ppy.sh/users/102335``), beatmapsets (``https://osu.ppy.sh/beatmapsets/611806#osu/1291369``), and any other view which has a fully functioning implementation in osu-web.

If unsure, ask a reviewer.


