# recently-updated-pages-custom
This WordPress plugin adds a widget with the ability to insert a list of recently updated posts or pages. It includes a shortcode [rup_display_update_date] to add an updated date in a post or you can use it in a template. 

See this in action on most of the pages of https://fyxtrpg.com/ . Look to the footer near the search widget. It will display the most recently updated pages on the website. (Post or Pages that have been edited and updated.)

This is an updated version of the original unmaintained plugin: https://wordpress.org/plugins/recently-updated-pages/

=== Recently Updated Pages ===

Contributors: Troy Whitney New Author, Original Author Ehsanul Haque

URI: http://www.imageinnovationsllc.com/

Tags: updated, recent, page, post

Requires at least: 2.8

Tested up to: 4.9.8

Stable Tag: 1.1.0


Add a widget to display a list of pages (and optionally posts) on WordPress that have been recently updated. It also lets you use WP's shortcodes to display last update date of the page or blog posts. 


== Description ==
Let your visitors know what content on your WordPress site has been recently updated with this easy to use widget. This widget can be added to any widget area and will dispay what pages and posts you've recently updated along with the date they were updated. There are a handful of display options you can set to fine tune exactly what is shown. 

Ability to choose if you want pages, posts, or both displayed.

Ability to choose if you would like to exclude pages, posts, or both. 

Add the shortcode [rup_display_update_date] to any page or post you would like to have the updated date added to. 

Use this plugin to enhance your own templates. 


== Installation ==
This plugin can be installed by the standard plugin installation process.

1. Upload folder containing `recently_updated_pages.php` and 'readme.txt to the `/wp-content/plugins/` directory.
2. Activate the plugin through the 'Plugins' menu in WordPress.
3. Go to `Widgets` section under `Appearance` menu.
4. Drag the `Recently Updated Pages` widget into the `Available Widgets` section.
5. Enter your desired options into the widget box or leave the default settings.
6. Save the widget changes. 


== Frequently Asked Questions ==

= 
What if I keep the title blank? 
=
By default the widget will show "Recently Updated Pages" as the title. If you want to display a different title, type it in and save.

= 
How many pages will it show in the list? 
=
You can define it through the widget editor in the Wordpress admin panel. Specify the number and save.

= 
Will I be able to show my blog POST titles in the list? 
=
Yes, now you can. Check the option to include the blog Posts in the list and it will show them along with the Page list.

=
Is there a way to hide the last update date? 
=
Yes, you can do that. Toggle the checkbox to hide or display the date. 

=
Can I change the date format? 
= 
There is now a text box to specify the date format. There's also a small help below the admin form in the Widget section.

=
How do I use the shortcode? 
=
There are two ways you can use it. Either by modifying the template files (e.g. single.php or page.php or footer.php) of the currently running theme or you can add the shortcode within the blog post or page through the WP admin post/page editors. 

To use the shortcode within the template file add the following PHP code:
&lt;&#63;php echo do_shortcode('[rup_display_update_date]'); &#63;&gt;

To use the shortcode through the post/page editor:
[rup_display_update_date]

= 
Can I control the date/time format for the shortcode?
=
Yes, you can. Through the widget settings (WP Admin > Appearance > Widgets > Recently Updated Pages) you can now control the date/time format for shortcodes.

= 
I'm trying to display the update date/time like 20th Aug 2010 at 5:30pm, but the word "at" shows up like "pm31". Why?
=
Because PHP's date function will recognize the characters "a" and "t" as format parameters and parse them. In order to show the word "at" you will need to escape both characters like "\a\t". 


== Changelog ==

= 
1.0.0 
=
* First release

= 
1.0.1 
= 
* Added feature to display list of recently updated blog Posts along with the pages

= 
1.0.2 
= 
* Added the feature to hide/display the update date
* Added the feature to specify the date format 

= 
1.0.3 
= 
* Added the feature to use shortcodes and control its date/time format

= 
1.0.4 
= 
* Bug fix: Fixed the admin panel widget area issue where any widget below RUP widget will lock up. 

=
1.1.0 
= 
* Added the ability to exclude posts and pages by entering their numbers in a new field on the widget. 
