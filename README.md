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
  <dd>Allow me to <a href="http://devtidbits.com/2011/03/16/the-wordpress-extended-rss-wxr-exportimport-xml-document-format-decoded-and-explained/">borrow a pretty simply definition</a>: "The WXR format is based on the Really Simple Syndication or RSS specification which is a very popular dialect of XML." Basically, it's an XML file very similar to an RSS feed you might get from any normal site to read its content elsewhere, which WordPress has extended with some of its own data to represent the content of a WordPress site.</dd>
  <dt>Why not provide a SQL file?</dt>
  <dd>I have considered this, and may do it (for reasons outlined below regarding limitations of WXR files). For the moment, I haven't done it mainly because of the additional dependencies and questions the SQL creates. Do I provide a full site dump? Then what if they don't have the default theme available? Do I only provide certain tables instead? How can I be sure I don't corrupt existing work in their site? I think eventually that will be a goal, but for the moment, this approach is working well enough.</dd>
  <dt>Do I need a plugin to use WPCF?</dt>
  <dd>Technically, yes. As mentioned in the installation instructions above, when you click on the "Import" option from the menu, WordPress will prompt you to install a plugin to import the data. This used to be first party functionality included by default in WordPress, but they moved it out into a plugin, I assume to lighten the package size of WordPress. This plugin is maintained by WordPress, however.</dd>
  <dt>Why are there broken links all over the site after importing?</dt>
  <dd>Make sure you do a find and replace in the XML file for http://localhost, and put in your site's domain. I left all pointers relatively generic for the folks working on a local machine, but if you're testing on an actual site or subdomain, you should make sure that's what's referenced in the code. If you can't handle doing a find/replace, then you probably shouldn't be doing whatever you're trying to do.</dd>
  <dt>What isn't supported by the WXR file?</dt>
  <dd>Well, obviously, no static media is included - images and such. All of the images you see are hotlinked from a placeholder image site. Also, and maybe most frustrating, is that so far they also don't represent menus in the WXR schema. So I can't give you example menus to test either, you'll have to make those on your own in your theme you're using.</dd>
</dl>

## Special Thanks
* WPCF makes use of http://www.fillmurray.com/ to provide example imagery on posts and pages, a product of [@davecowart](https://twitter.com/davecowart "Dave Cowart on Twitter").
* The markdown version of our Creative Commons license is based on the work of [Creative Commons Markdown](https://github.com/idleberg/Creative-Commons-Markdown) by [Jan T. Sott](https://github.com/idleberg).

- - -

![Creative Commons Attribution-ShareAlike 4.0 International](http://i.creativecommons.org/l/by-sa/4.0/88x31.png "Creative Commons Attribution-ShareAlike 4.0 International")
