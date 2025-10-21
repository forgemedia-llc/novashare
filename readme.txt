=== Novashare ===
Contributors:
Donate link: https://novashare.io
Tags: novashare
Requires at least: 5.5
Requires PHP: 7.0
Tested up to: 6.8.3
Stable tag: 1.6.3
License: GPLv2 or later
License URI: https://www.gnu.org/licenses/gpl-2.0.html

WordPress social sharing at the speed of light.

== Description ==

[Novashare](https://novashare.io/) is a simple, fast, and lightweight social sharing plugin developed from the ground up with a performance-focused approach to increase your shares. 

= Features =

* Blazing fast. Scripts don’t run where they shouldn’t and it uses inline SVG icons without the overhead of third-party libraries. There is no jQuery dependency, and no JS is loaded with basic setups.
* Easy UI with no admin menu clutter. Enable inline share buttons, floating, or both. Pick from 25+ different networks and match your site’s branding in seconds.
* Blocks for every feature, which enables on-the-fly previews and customization.
* Show off your most popular content by enabling share counts.
* Responsive and works on all devices, from desktops to mobile phones. Set breakpoints above and below where you want to hide your share buttons.
* Utilize extra features such as Pinterest hover pins, share window, highlight share, and link shortening.

= Documentation =

Check out our [documentation](https://novashare.io/docs/) for more information on how to use Novashare.

== Changelog ==

= 1.6.3 - 10.21.2025 =
* Added new AI share buttons for Claude and Google AI.
* Added new novashare_ai_network_text filter.
* Added support to set the Novashare license key via wp-config.php using the NOVASHARE_LICENSE_KEY constant.
* Removed Pocket share network from the plugin, as they have shut down.

= 1.6.2 - 08.25.2025 =
* Added new AI share buttons for ChatGPT, Grok, and Perplexity which link to a prompt that will summarize the shared post's content.
* Added follow button support for Nextdoor.
* Updated Nextdoor brand colors.
* Adjusted copy button URL to work with existing novashare_permalink filter when displayed on single posts.
* Fixed multiple PHP warnings coming from the follow widget class.
* Fixed an issue where floating bar icons were not centering properly when fill available space option was being used.
* Reverted Facebook share button mobile URL to use web link to be more compatible with all platforms.
* Updated our staging site license key exception list with additional formats.

= 1.6.1 - 06.30.2025 =
* Added new novashare_page_builders filter.
* Added new Pinterest image pin options for Image Placement to control which images get pin buttons added. The novashare_pinterest_image_excluded filter that was previously used for whitelisting will still work for the time being, but that will now be managed in the UI going forward.
* Started work on moving more universal style properties like button size and button margin to CSS variables.
* Refactored specific portions of the main frontend stylesheet, reducing the file size by 7.69%. We recommend that you clear all cache layers (Unused/Critical CSS, server cache, CDN cache) after updating.
* Cleaned up and removed redundant inline style overrides for inline content buttons.
* Adjusted admin UI JavaScript to allow for child options to have multiple controllers of different types.
* Fixed an issue where floating bar buttons were being added to the Bricks editor UI.
* Fixed an issue where Facebook share button was not working correctly on mobile.

= 1.6.0 - 04.10.2025 =
* Added share button support for Nextdoor network.
* Added new Total Share Count and Network Share Count options to share button section with additional frontend styles to display the total share count at the top of the share window.
* Adjusted total share count calculations to display the combined total regardless of network selection if the share button is being used.
* Deployed a secondary API that can be used when the client has issues communicating with our licensing server (usually due to firewalls).

= 1.5.9 - 03.05.2025 =
* Added new location follow button.
* Added support for image pin buttons to appear on images inside Bricks editor content.
* Added dynamic label font size for follow buttons relative to the overall size set for the buttons.
* Fixed an issue where the follow block height would not always display correctly in the editor.
* Fixed a display error that could sometimes happen with certain follow block networks.
* Fixed an issue where Pinterest image content was returning blank when no global post data was available.
* Fixed multiple display issues with highlight buttons that could happen with specific setups.
* Moved the show on scroll load event to an event listener to prevent conflicts with other onload events.
* Updated our staging site license key exception list with additional formats.

= 1.5.8 - 01.28.2025 =
* Added new Show Labels control to the follow buttons block.
* Updated all blocks to API version 3 to support rendering the block inside the post editor iframe.
* Fixed multiple deprecated UI element warnings showing up in the block editor.
* Fixed a missing anchor link pointing to the license tab in our plugin settings UI.
* Fixed an issue where additional CSS classes set in the advanced section of the share buttons block were not added to the HTML output.
* Fixed an encoding issue with certain Pinterest descriptions when added to page images for the image grid via JavaScript.
* Some minor code refactoring and style cleanup.
* Removed trailing empty block style in the main stylesheet that was previously used to fix a block editor enqueuing issue.

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
