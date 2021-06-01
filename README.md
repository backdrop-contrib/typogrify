Typogrify
======================

Brings the typographic refinements of *Typogrify* to Backdrop CMS:

* Wraps ampersands (the "&" character) with `<span class="amp">&amp</span>`.

* Prevents single words from wrapping onto their own line using Shaun Inman's
  Widont technique.

* Converts straight quotation marks to typographer's quotation marks, using
  SmartyPants.

* Converts multiple hyphens to en dashes and em dashes (according to your
  preferences), using SmartyPants.

* Wraps multiple capital letters with `<span class="caps">CAPS</span>`.

* Wraps abbreviations with `<span class="abbr">t.l.a.</span>`.

* Wraps initial quotation marks with `<span class="quo"></span>` or
  `<span class="dquo"></span>`.

* Adds a css style sheet that uses the `<span>` tags to substitute a showy
  ampersand in headlines, switch caps to small caps, and hang initial quotation
  marks.

Typogrify is a collection of Text filters for Django that help prettify web
typography by preventing ugly quotes and widows, and providing CSS hooks to
style some special cases.


Requirements
------------

 * none


Installation
------------

- Install this module using the official Backdrop CMS instructions at
  https://backdropcms.org/guide/modules.

- Visit the configuration page under Administration > Configuration >
  Content authoring > Text editors and Formats (admin/config/content/formats)
  and then click 'configure' next to the format you'd like to use.
  * For starters, you probably just want to add this filter to your default
    input format.
  * Typogrify expects html input so it should be be the last filter you apply
    (ie, after Markdown).
  * Typogrify will not work as expected if it is applied to plain text, or if it
    is the only filter applied to the text.

- Choose which typographic refinements to apply


Documentation
-------------

Additional documentation is located in the Wiki:
https://github.com/backdrop-contrib/typogrify/wiki/Documentation.

Issues
------

Bugs and Feature requests should be reported in the Issue Queue:
https://github.com/backdrop-contrib/typogrify/issues.

Current Maintainers
-------------------

- [Jen Lampton](https://github.com/jenlampton).
- Seeking additional maintainers.

Credits
-------

- Ported to Backdrop CMS by [Jen Lampton](https://github.com/jenlampton).
- Backdrop port sponsored by [Ivar Jacobson International](https://www.ivarjacobson.com)
- Maintained for Drupal by [many wonderful contributors](https://www.drupal.org/node/149970/committers).
- Originally written for Drupal by [Derek Wright](https://www.drupal.org/u/dww).
- The original Typogrify is Python code by [Christian Metts](https://github.com/mintchaos).
- PHP port of Python code, php-typogrify, by [Hamish Macpherson](https://github.com/hamstu).
- Original [Typogrify project page](http://code.google.com/p/typogrify/)
- Typogrify.module uses [PHP SmartyPants](http://www.michelf.com/projects/php-smartypants/)
- Typogrify.module implements [Widont](http://www.shauninman.com/archive/2006/08/22/widont_wordpress_plugin)

License
-------

This project is GPL v2 software.
See the LICENSE.txt file in this directory for complete text.

