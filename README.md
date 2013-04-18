Wordpress Content Framework
===========================

The WCFW is a Wordpress generated WXR (WordPress eXtended RSS) file generated with a complete set of sandbox data that you can use for theme, plugin, CSS, or other development that requires you to have a broad set of sample data to work from. This particular file contains information about a site's posts, pages, comments, categories, menus, and other content.

Compatibility
=============
WCFW 2.0 was generated for Wordpress 3.5.1. It may work with older or newer versions of Wordpress as well.

Installation
============
To import this information into a WordPress site follow these steps:
0. If you aren't running your version of Wordpress on localhost, you may want to do a find/replace on the WXR file for http://localhost and put in your domain.
1. Log in to that site as an administrator.
2. Go to Tools: Import in the WordPress admin panel.
3. Install the "WordPress" importer from the list (Wordpress will attempt to download and install a plugin for this, it's okay).
4. Activate & Run Importer.
5. Upload this file using the form provided on that page.
6. You will first be asked to map the authors in this export file to users on the site. For each author, you may choose to map to an existing user on the site or to create a new user. By default, it should try to just map them to 'admin.'
7. WordPress will then import each of the posts, pages, comments, categories, etc. contained in this file into your site.