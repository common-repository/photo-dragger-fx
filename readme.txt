=== Photo Dragger FX ===
Contributors: flashxml
Tags: images, photos, widget, post, plugin, posts, sidebar, free, flash, photo, drag, image, as3, effects, vertical, horizontal, text, xml, html, css, scroll, dragger
Requires at least: 2.8.0
Tested up to: 3.0.1
Stable tag: trunk

An original Photo Dragger. Completely XML customizable, without any Flash knowledge. And it's free!

== Description ==

You can integrate it in any website for free without any Flash knowledge. It has customizable width and height, it uses HTML/CSS formatted text and has the possibility for vertical/horizontal position. The configurable reflection, the multiple roll over/out effects and configurable reflection are the other features of this product. Many other options are available in the Live Demo.

== Installation ==

Make sure your Wordpress version is greater than 2.8 and your hosting provider is using PHP5.

1. There are two files to download: [WordPress Plugin](http://downloads.wordpress.org/plugin/photo-dragger-fx.zip "Photo Dragger FX Plugin") (that you have to install and activate) & [Free package](http://www.flashxml.net/free/download/photo-dragger.zip "Photo Dragger FX")
2. Create a new folder inside your **wp-content** folder called **flashxml**, inside this folder create a new one called **photo-dragger-fx** and copy the content of the **free package** there
3. If you copied the **free package** to a location different than the one above, go to **Photo Dragger FX** from the **Settings** tab in your **WordPress Dashboard** and update the path accordingly
4. Add `[photo-dragger-fx][/photo-dragger-fx]` where you want the Flash to show up in your post/page
5. If you want to make the Photo Dragger FX part of your theme, edit the template files and add `<?php photodraggerfx_echo_embed_code(); ?>` where you want it to show up
6. Go to [FlashXML.net](http://www.flashxml.net/ "Free Flash Components") and [customize your Photo Dragger FX](http://www.flashxml.net/photo-dragger.html "Photo Dragger FX") using the Live Demo. Generate the `settings.xml` text and use it to overwrite `wp-content/flashxml/photo-dragger-fx/settings.xml`
7. To use your own images, upload them to `wp-content/flashxml/photo-dragger-fx/images/` and update the `wp-content/flashxml/photo-dragger-fx/images.xml` file accordingly

= Additional settings file =

To embed the Photo Dragger FX more than once, you will need another settings file and (probably) another set of images. Let's assume your new file is called `settings2.xml`. Add `[photo-dragger-fx settings="settings2.xml"][/photo-dragger-fx]` where you want the Flash to show up in your post/page. If you made the Flash part of your theme, add the file name as **the first argument** of the `photodraggerfx_echo_embed_code()` function call (for example `<?php photodraggerfx_echo_embed_code("settings2.xml"); ?>`).

= No Flash support text =

To support visitors without Adobe Flash Player, you can provide alternative content by adding the text between `[photo-dragger-fx]` and `[/photo-dragger-fx]`. If you made the Flash part of your theme, add the text as **the second argument** of the `photodraggerfx_echo_embed_code()` function call (for example `<?php photodraggerfx_echo_embed_code("","Alternative content"); ?>`).

= If you have PHP4 =

To make it work with PHP4, add `[photo-dragger-fx width="600" height="300"][/photo-dragger-fx]` where you want the Flash to show up in your post/page. If you made the Flash part of your theme, add the width and height as **the third and fourth argument** of the `photodraggerfx_echo_embed_code()` function call. Don't forget to provide your own width and height values, since 600 and 300 are just examples.

= Getting rid of the FlashXML.net label =

To remove the FlashXML.net label from the top-left corner you'll need to buy the [paid package](http://www.flashxml.net/photo-dragger.html "Photo Dragger FX"). Once you'll do that, simply use the SWF file from the paid package to overwrite the SWF file from the `wp-content/flashxml/photo-dragger-fx/` folder.

== Screenshots ==

1. The Live Demo on [FlashXML.net](http://www.flashxml.net/photo-dragger.html "Photo Dragger FX") is the utility that helps easily customize your Photo Dragger FX to fit all your needs.