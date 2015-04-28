---
layout: page
title: API
permalink: /api/
---

The Pair Columbus API is a public, read-only resource for information related to the group and its resources. For now, it just serves static JSON used to generate the [Challenges page](/challenges/).

## [Challenges](/api/challenges.json)
This endpoint returns all active Pair Columbus challenges in categories (generally based on difficulty or technologies used).

### Request
`GET http://paircolumbus.org/api/challenges.json`

### Response
__200 (application/json)__

Returns an array of Categories.

#### Category
category
: The name of the category.

description
: One or more sentences describing the intention of the challenges in the category. Note that some descriptions contain [Markdown](http://daringfireball.net/projects/markdown/) content, so you may need to render them with a Markdown parser first.

challenges
: A list of strings of challenge names. Each challenge is named exactly after the name of its repository in the [Pair Columbus GitHub Organization](https://github.com/paircolumbus). To get the URL of a challenge's repository, prepend `https://github.com/paircolumbus/` to its name.

#### Example
This example is a subset of the real results, and has added whitespace for readability.

{%highlight json%}
[
  {
    "category": "Beginner",
    "description": "For beginners to programming.",
    "challenges": [
      "Git-It",
      "RubyRefresher"
    ]
  }
]
{%endhighlight%}
