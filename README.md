# WordPress Content Framework

The WPCF is a WordPress generated WXR (WordPress eXtended RSS) file generated with a complete set of sandbox data that you can use for theme, plugin, CSS, or other development that requires you to have a broad set of sample data to work from. This particular file contains information about a site's posts, pages, comments, categories, menus, and other content.

## Compatibility
WPCF 2.4 was generated for WordPress 4.1.1. It may work with older or newer versions of WordPress as well. In general, the standard WordPress uses for its WXR file is consistent enough that it's not extremely version specific. Unsupported data will usually just be ignored in older versions.

### Master vs. Tags
You can always [download the latest tagged release](https://github.com/thequicksilver/wordpress-content-framework/releases) on our GitHub page. However, you should normally be able to download the latest copy of the [Master branch](https://github.com/thequicksilver/wordpress-content-framework/tree/master) and still have no issues. Commits pulled into Master before a release should be stable enough for general use. More likely than not, commits pulled into Master before a tag will usually just have to do with typos and simple things like that. The [Development branch](https://github.com/thequicksilver/wordpress-content-framework/tree/development), on the other hand, is never guaranteed to be stable, but hey, feel free to live dangerously if you like.

## Installation
To import this information into a WordPress site follow these steps:

![Import tool in the WordPress back end](http://i62.tinypic.com/32zuo9g.jpg "Import tool in the WordPress back end")

1. If you aren't running your version of WordPress on localhost, you may want to do a find/replace on the WXR file for http://localhost and put in your domain.
2. Log in to that site as an administrator.
3. Go to Tools: Import in the WordPress admin panel.
4. Install the "WordPress" importer from the list (WordPress will attempt to download and install a plugin for this, it's okay).
5. Activate & Run Importer.
6. Upload this file using the form provided on that page.
7. You will first be asked to map the authors in this export file to users on the site. For each author, you may choose to map to an existing user on the site or to create a new user. By default, it should try to just map them to 'admin.'
8. WordPress will then import each of the posts, pages, comments, categories, etc. contained in this file into your site.

## Frequently Asked Questions
<dl>
  <dt>What is a WXR File?</dt>
  <dd></dd>
  <dt>Why not provide a SQL file?</dt>
  <dd></dd>
  <dt>Do I need a plugin to use WPCF?</dt>
  <dd></dd>
  <dt>Why are there broken links all over the site after importing?</dt>
  <dd></dd>
  <dt>What isn't supported by the WXR file?</dt>
  <dd></dd>
</dl>

## Special Thanks
* WPCF makes use of http://www.fillmurray.com/ to provide example imagery on posts and pages, a product of [@davecowart](https://twitter.com/davecowart "Dave Cowart on Twitter").
* The markdown version of our Creative Commons license is based on the work of [Creative Commons Markdown](https://github.com/idleberg/Creative-Commons-Markdown) by [Jan T. Sott](https://github.com/idleberg).

- - -

![Creative Commons Attribution-ShareAlike 4.0 International](http://i.creativecommons.org/l/by-sa/4.0/88x31.png "Creative Commons Attribution-ShareAlike 4.0 International")
