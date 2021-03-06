Simple DKI
==========

Quick and Dirty Dynamic Keyword Injection with Shortcode

If a Page has a URL argument `keyword={keyword}` or `kw={keyword}` the Plugin automagically overwrites the default WordPress Page `the_title()` and Header `<title>` with that `{keyword}`. Multiple words can be separate by a `+` character which is converted to spaces upon output.

Also provides a `[keyword]` shortcode for Dynamic Keyword Injection in to Page / Post / Widget / whatever content, which has the following arguments:

* case :
  * "titlecase" (default) uses ucwords(...) to Title Case whatever keyword(s) are present
  * "upper" or "uppercase"
  * "lower" or "lowercase"
* default
  * defaults to "" which will not override the default Page Title wherever it may appear, but will just not output anything when the shortcode is used.
  * optionally specify a word or phrase to output if a keyword or kw is found present in the URL

Installation
------------

0. Upload file to the `/wp-content/plugins/` directory
0. Activate the Simple DKI plugin through the 'Plugins' menu in the WordPress Admin Panel.
0. Use the shortcode on any Pages you want
0. Link people to those pages with the kw or keyword URL arguments

Changelog
---------

### 1.0.1

Updated author, author URI, and License in the Plugin info

### 1.0

Initial release
