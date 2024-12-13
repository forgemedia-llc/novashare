=== Novashare ===
Contributors:
Donate link: https://novashare.io
Tags: novashare
Requires at least: 5.5
Requires PHP: 7.0
Tested up to: 6.7.1
Stable tag: 1.5.7
License: GPLv2 or later
License URI: https://www.gnu.org/licenses/gpl-2.0.html

WordPress social sharing at the speed of light.

== Description ==

[Novashare](https://novashare.io/) is a simple, fast, and lightweight social sharing plugin developed from the ground up with a performance-focused approach to increase your shares. 

= Features =

* Blazing fast. Scripts don’t run where they shouldn’t and it uses inline SVG icons without the overhead of third-party libraries.
* Easy UI with no admin menu clutter. Enable inline share buttons, floating, or both. Pick from 25+ different networks and match your site’s branding in seconds.
* Show off your most popular content by enabling share counts.
* Responsive and works on all devices, from desktops to mobile phones. Set breakpoints above and below where you want to hide your share buttons.
* Utilize extra features such as Pinterest hover pins, share window, and link shortening.

= Documentation =

Check out our [documentation](https://novashare.io/docs/) for more information on how to use Novashare.

== Changelog ==

= 1.5.7 - 12.13.2024 =
* Added new conditional inline JavaScript to dynamically add Pinterest descriptions to content images when using the image grid.
* Made some adjustments to content marker function to share between different features.
* Fixed an issue where percentage dimension values were flagging as below the minimum threshold for a Pinterest image pin button.
* Fixed an issue with WordPress 6.7.1 where the text domain for translations was loading too early.
* Removed older changelog entries in readme.txt file and added link to web version.

= 1.5.6 - 10.24.2024 =
* Added new Highlight feature which allows for sharing of highlighted text in page and post content to supported networks.
* Adjusted aria-label attributes throughout the plugin to be more specific to element actions.
* Fixed an issue where the inline JavaScript wasn't printing correctly if only the floating bar was being used on the page.
* Fixed the missing plugin UI color for the Hacker News network.
* Fixed an issue where Pinterest image buttons were displaying incorrectly if there was another pinit.js script loading on the site.
* Fixed an issue with the logo scaling in the plugin UI on smaller devices.
* Translation updates.

= 1.5.5 - 09.27.2024 =
* Fixed an issue where image pin links were not opening correctly when sharing a single image.
* Fixed multiple minor image pin styling issues.

= 1.5.4 - 09.26.2024 =
* Added share and follow button support for Bluesky network.
* Updated share button functionality to now open in a new browser tab instead of a popup window for relevant networks. This allows us to completely remove the frontend Novashare JavaScript file which is no longer needed with these changes. Pinterest-specific JavaScript to manage the image grid will now be printed inline when needed.
* Optimized plugin logo and inline SVG network icons.
* Fixed an issue where the license tab was showing up at the subsite level if the plugin was not network activated in a multisite environment.
* Fixed an issue where X share button was not handing off to the native app when on a mobile device.
* Fixed an issue where a blank tab would sometimes be left behind in the browser on mobile when handing off to a native app.
* Removed deprecated API calls for TwitCount and OpenShareCount.
* Updated Grow references to Hubbub in the Novashare Migrator.

= 1.5.3 - 08.06.2024 =
* Fixed an issue where the old Twitter domain link was redirecting and duplicating the query string parameters passed through.
* Added an additional post object check to prevent a PHP warning in certain cases.
* Updated our staging site license key exception list with additional formats.
* Minor style adjustments to the plugin UI.

= 1.5.2 - 07.16.2024 =
* Added Pinterest Description fields back throughout the plugin which will tie directly to the description parameter shared on Pinterest links to help with internal search.
* Updated our staging site license key exception list with additional formats.
* Minor style adjustments to the plugin UI.
* Moved from using global $post variable to pulling from the queried object to prevent conflicts with other plugins.
* Removed certain rel attribute values from links that are no longer needed for modern browsers.

= 1.5.1 - 05.24.2024 =
* Updated our staging site license key exception list with additional formats.
* Fixed an issue with image pins where the first image in the post would be shared instead of the image that was clicked on.
* Fixed an issue where the open graph image would sometimes show up in the image grid even when the behavior was set to show only Pinterest images.
* Fixed an issue where field validation was preventing some Mastodon username formats from being entered.

= 1.5.0 - 05.01.2024 =
* Added new option to control Image Pin Button Behavior with additional options to share the post image or show the image grid.
* Added new Image Grid Behavior option.
* Adjusted current share button behavior options to reflect image grid changes.
* Added share button support for Threads network.
* Added lodash dependancy to Pinterest block editor script in the admin.
* Fixed an undefined index warning coming from functions.php.

= 1.4.9 - 03.31.2024 =
* Added new configuration option to add a Mastodon Username which will be added to the content of the post when shared.
* Added new open graph integration for Rank Math SEO.
* Fixed an issue that was causing an empty share block to throw an error in the block editor after saving the post.
* Fixed an issue where hidden Pinterest images were showing thumbnail resolution versions when shared.
* Fixed an open graph issue with SEOPress integration that was using the wrong filters for the main title and description tags.
* Fixed a typo in the inline SVG code for the X network.

= 1.4.8 - 01.31.2024 =
* Added new Custom option to Follow Button block along with controls to add your own inline SVG HTML and background color.
* Added new Pinterest option to Always Show image pin buttons instead of only on hover.
* Added additional Pinterest image pin styles to help with compatibility when placed inside aligned containers.
* Fixed an issue with image pin button links not working with relative URLs.
* Fixed an issue in the plugin settings UI where textarea inputs were not sizing down correctly.

View the full changelog:
[https://novashare.io/docs/changelog/](https://novashare.io/docs/changelog/)
