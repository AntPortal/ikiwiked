#Ikiwiked



A collection of themes, templates, and wiki directive pages for [ikiwiki](http://ikiwiki.info). For an example of the theme, look at [antportal](https://antportal.com/wiki)


##Content


### Templates

Directory containing templates that are not shipped with ikiwiki. We use this template to manage our TODOs (as an issue tracker, see [ikiwiki issue tracker](http://ikiwiki.info/tips/integrated_issue_tracking_with_ikiwiki/]] for justification)).

### Theme

Directory containing themes (both [SASS](http://sass-lang.com/) files and complied CSS, the last one for convenience only). 

local.css is the modified version that makes ikiwiki look better (in my opinion).
local.scss is the source file used (see [sass](http://sass-lang.com/) how to obtain the compiler).

### Test

Directory containing an example that can be used to tweak/configure your own theme. style.css comes with ikiwiki. To use a specific theme, copy the .scss theme into this directory (or .css if you prefer), run sass (or not) and visit wiki.html to test.


##Installation



The bare minimum is given here. For a much more indepth and comprehensive installation instructions got the source: [ikiwiki](http://ikiwiki.info).

###Templates

Move the template to your template directory. For example,

     <pre>/usr/share/ikiwiki/templates/titleandtags.tmpl</pre>

For template usage, see [ikiwiki templates](http://ikiwiki.info/ikiwiki/directive/template/).

###Theme

Move the local.css to your theme directory. For example (if you don't want to modify your ikiwiki.setup file) you can move it (and override the presumably empty) to

     <pre>/usr/share/ikiwiki/basewiki/local.css</pre>

Finally, run <code>sudo ikiwiki --setup /etc/ikiwiki/ikiwiki.setup</code>