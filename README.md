# jekyll-social-metatags
A simple Jekyll include file to add metadata tags for search engines and social networks to better index and display your site's content. No plugin required.

## Installation

Just place the `social-metatags.html` into your `_includes` folder and add this before your `</head>` html tag:
```
{% include social-metatags.html %}
```

## Usage

The metatags of any of the following fields will be created, if included in your site's `_config.yml`:

```
description:
author:
featured_image:
twitter:
  username:
  site:
facebook:
  app_id:
  publisher:
  admins:
```

The metatags of any of the following fields will override the site's ones, if included in your post/page file:

```
title:
author:
twitter_username:
facebook_publisher:
keywords:
tags:
categories:
category:
featured_image:
date:
modified_date:
```
