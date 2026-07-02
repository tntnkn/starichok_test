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
show_author:
show_practice_block:
show_contact_form:
canonical_url:
seo_title:
seo_description:
```

Forms are visual-only in this version. Submission wiring is intentionally deferred.
