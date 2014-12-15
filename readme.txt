=== Random Posts from Category ===
Contributors: sillybean
Tags: widget, random, posts
Donate link: http://stephanieleary.com/code/wordpress/random-posts-from-category/
Text Domain: RandomPostsFromCategory
Domain Path: /languages
Requires at least: 2.8
Tested up to: 4.1
Stable tag: 1.2

A widget that lists random posts from a chosen category.  

== Description ==

This widget will list random posts from a chosen category. You can choose how many posts to display, and whether to show the excerpt or the full content in addition to the post title. You may also link the widget title to the category archive if you like.

== Translations ==

Belorussian (be_BY) by <a href="http://fatcow.com">FatCow</a>.
Romanian (ro_RO) by Web Geek Science (<a href="http://webhostinggeeks.com/">Web
Hosting Geeks</a>)

If you would like to send me a translation, please write to me through <a href="http://sillybean.net/about/contact/">my contact page</a>. Let me know which plugin you've translated and how you would like to be credited. I will write you back so you can attach the files in your reply.

== Installation ==

1. Upload the plugin directory to `/wp-content/plugins/` 
1. Activate the plugin through the 'Plugins' menu in WordPress

Go to Appearance &rarr; Widgets to add widgets to your sidebar in widget-ready themes.

To use with a custom post type, add this to your post type plugin file or theme functions.php:

`
add_filter('random_posts_from_category_args', 'random_post_widget_args');

function random_post_widget_args($args) {
	$args['post_type'] = 'mycpt_name';
	return $args;
}
`

== Screenshots ==

1. The widget

== Changelog ==

= 1.2 =
* Added 'random_posts_from_category_args' filter to query arguments; fixed query reset.
= 1.16 =
* Romanian (ro_RO) translation by Web Geek Science (<a href="http://webhostinggeeks.com/">Web
Hosting Geeks</a>)
= 1.15 =
* Fixed an HTML problem with linked titles. (Thanks, Anthony Eden!)
= 1.14 =
* Added options to display content or excerpt without the title (November 5, 2010)
= 1.13 =
* Fixed a bug where the dropdown would turn into plain text after saving options. (November 18, 2009)
= 1.12 =
* Belorussian (be_BY) translation by <a href="http://fatcow.com">FatCow</a>. (November 15, 2009)
= 1.11 =
* Fixed a bug with the dropdown options (November 14, 2009)
= 1.1 =
* Internationalization improvements (November 13, 2009)\
= 1.0 =
* First release (August 6, 2009)