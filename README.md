# Jekyll Blog Theme

Standalone Jekyll theme prototype for `blog.milsky-advokat.ru`.

## Local Setup

Ruby, Bundler, and Jekyll are not currently installed in this workspace environment. On Windows, install Ruby with DevKit first, then run:

```powershell
gem install bundler
bundle install
bundle exec jekyll serve --livereload
```

The local site will be available at:

```text
http://127.0.0.1:4000/
```

## Content Model

Posts live in `_posts/` as Markdown files. Each post supports:

```yaml
title:
description:
eyebrow:
slug:
date:
image:
category:
author:
show_author:
show_practice_block:
show_contact_form:
canonical_url:
seo_title:
seo_description:
```

Categories are listed in `_data/categories.yml`. The `title` value must match a post's `category` front matter exactly; `slug` controls the generated category URL under `/categories/<slug>/`.

Authors are listed in `_data/authors.yml`. Posts can set `author` to an author ID, for example `milskiy-andrey`; omitted values fall back to `default_author` in `_config.yml`. Author pages live under `/authors/<slug>/`.

Forms are visual-only in this version. Submission wiring is intentionally deferred.
