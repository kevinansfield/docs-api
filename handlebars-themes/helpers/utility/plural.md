---
title: "plural"
tags:
    - api
    - handlebars
    - themes
    - helpers
---

Usage: `{{plural value empty="" singular="" plural=""}}`

### Description

`{{plural}}` is a formatting helper for outputting strings which change depending on whether a number is singular or plural.

The most common use case for the plural helper is outputting information about how many posts there are in total in a collection. For example, themes have access to `pagination.total` on the homepage, a tag page or an author page.

You can override the default text, [see translate the plural helper](/docs/i18n#section-plural-helper). 

### Examples

```
{{plural pagination.total empty='No posts' singular='% post' plural='% posts'}}
```

`%` is parsed by Ghost and will be replaced by the number of posts. This is a specific behaviour for the helper.