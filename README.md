# jekyll-social-metatags

A simple Jekyll include file to add metadata tags for search engines and social networks to better index and display your site's content. No plugin required.

It adds the following meta tags to your site:

* Page title
* Page description
* Canonical URL
* [Open Graph](http://ogp.me/) title, description, site title, and URL (for Facebook, LinkedIn, etc.)
* [Twitter Summary Card](https://dev.twitter.com/cards/overview) metadata

## Installation

Just place the `social-metatags.html` into your `_includes` folder and add this before your `</head>` html tag:
```
{% include social-metatags.html %}
```

## Usage

The metatags of any of the following fields will be created, if included in your site's `_config.yml`:

* `title` - Your site's title (e.g., Ben's awesome site, The GitHub Blog, etc.)
* `description` - A short description (e.g., A blog dedicated to reviewing cat gifs)
* `image` - URL to an image associated with the website (e.g., `/assets/screenshot-jumbo.png`)
* `author` - global author information (see below)
* `twitter:username` or `twitter:site` - The author/site's Twitter handle. You'll want to describe it like so:

  ```yml
  twitter:
    username: personal_handle
    site: publisher_handle
  ```

* `facebook` - The following properties are available:
  * `facebook:app_id` - a Facebook app ID for Facebook insights
  * `facebook:publisher` - a Facebook page URL or ID of the publishing entity
  * `facebook:admins` - a Facebook user ID for domain insights linked to a personal account

  You'll want to describe one or more like so:

   ```yml
  facebook:
    app_id: 1234
    publisher: 1234
    admins: 1234
   ```

The metatags of any of the following fields will override the site's ones, if included in your post/page file:

* `title` - The title of the post, page, or document
* `description` - A short description of the page's content
* `image` - URL to an image associated with the post, page, or document (e.g., `/assets/page-pic.jpg`)
* `author` - Page-, post-, or document-specific author information (name)
* `twitter:username` - The site's Twitter handle. You'll want to describe it like so:
* `facebook` - The following properties are available:
  * `facebook:publisher` - a Facebook page URL or ID of the publishing entity
* `keywords`, `tags`, `categories`, `category` - Page-, post-, or document-specific keywords information
* `date` - Page-, post-, or document-specific publishing date
* `modified_date` - Page-, post-, or document-specific modified date
