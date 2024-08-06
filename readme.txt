=== Novashare ===
Contributors:
Donate link: https://novashare.io
Tags: novashare
Requires at least: 5.5
Requires PHP: 7.0
Tested up to: 6.6.1
Stable tag: 1.5.3
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

= 1.4.7 - 12.13.2023 =
* Added input placeholder values for text fields in analytics settings section.
* Added Perfmatters discount link to plugin settings UI for Novashare customers.
* Updated Threads follow link UI behavior to expect a full URL instead of just a username to match other networks. If you have an existing Threads follow button placed on your site, you will need to update the link value.
* Fixed an issue where click to post theme and CTA position settings could not be set to a default value at the block level if a global value was already set.
* Fixed an issue where click to post inline styles would not print correctly in some cases.
* Added support for Social Snap to the Novashare Migrator.

= 1.4.6 - 10.18.2023 =
* Added Mastodon network support for Share and Follow Buttons.
* Added Threads network support for Follow Buttons.
* Updated Pinterest recommended image size in post meta options.
* Fixed an issue where the share window call to action was printing twice when set to a custom string.
* Fixed a PHP warning from meta.php that was showing up on the comment edit screen.
* Added the Novashare Migrator to work with latest AJAX changes to the settings UI.

= 1.4.5 - 09.18.2023 =
* Reworked the majority of the UI to use WordPress AJAX to save data and perform plugin actions.
* Updated Twitter branding to X.
* Fixed an issue where duplicate images on a page were getting Pinterest image hover buttons applied multiple times.
* Fixed an issue where the main stylesheet was not getting loaded when using the Full Site Editor.
* Fixed an issue where the Click to Post block was not showing up on a fresh install of the plugin.

= 1.4.4 - 07.26.2023 =
* Added new Share Buttons Block, which allows for on-the-fly customization of share buttons and the ability to easily place them anywhere.
* Fixed an issue where the default background color was sometimes not getting applied to the Pinterest image pin buttons.
* Fixed multiple undefined index warnings coming from meta.php.
* Removed Global Styles option and associated conditional stylesheet loading functionality to ensure site-wide block support.

= 1.4.3 - 06.15.2023 =
* Added new Pinterest image pin options for Button Color and Icon Color.
* Added new novashare_pinterest_image_excluded_filters filter.
* Added new logic to display an inline message if global styles are needed for a block to display correctly.
* Fixed an issue that was preventing the icon hover color from showing up in certain cases.
* Fixed an encoding issue with the copy button alert function.
* Fixed an issue where the main stylesheet was loading in some instances where it didn't need to be.

= 1.4.2 - 05.09.2023 =
* Added new Icon Color and Icon Hover Color options to both Inline Content and Floating Bar sections.
* Fixed an issue where accessibility mode tooltips were not getting styled properly in the plugin UI.

= 1.4.1 - 04.18.2023 =
* Added new Pinterest option to Enable Image Attributes to allow for control throughout the plugin, even if image pins are not enabled.
* We are deprecating the Pinterest title and description fields throughout the plugin, as Pinterest has moved to using Open Graph data instead of passing specific data through the individual links. For the time being, existing data will still be preserved and can be accessed by using our new novashare_show_deprecated filter.
* Added logic to print Pinterest image pin inline styles with the main stylesheet when global styles are turned on.
* Removed customer email row from the license tab.
* Style adjustments made for admin notices and main containers.
* Fixed an issue where image pins were not getting the correct src set with certain lazy loaders active.
* Fixed a styling issue in Safari where the settings UI logo was getting clipped.
* Fixed a styling issue where link and button colors were getting applied outside of the main Novashare admin container.

= 1.4.0 - 03.22.2023 =
* Updated the multisite network settings page to match the new UI.
* Added alt tags to Pinterest hidden images to fix validation issue.

= 1.3.9 - 03.15.2023 =
* Updated plugin settings UI. Completely overhauled admin header and navigation. Made additional improvements to various elements (icons, buttons, toggles, etc.).

= 1.3.8 - 02.13.2023 =
* Replaced all uses of .novashare- class prefixes to .ns- in front-facing CSS to improve performance (minified stylesheet reduced by 20%).

**IMPORTANT:** Due to the majority of all Novashare CSS classes being changed, we recommend that you clear all cache layers (Used/Critical CSS, server cache, CDN cache) after updating. Any custom code related to Novashare buttons will also need to be updated. Please reach out if you have any questions. We're happy to help.
* Added new novashare_pinterest_hidden_images filter.
* Added notice to plugin update row if there is not an active license key.
* Updated license key field to prevent it from getting auto-filled by browser extensions.

= 1.3.7 - 01.23.2023 =
* Fixed an issue where custom button colors were not getting applied correctly.

= 1.3.6 - 01.05.2023 =
* Switched to using CSS variables for various network colors to improve performance (minified stylesheet reduced by 19%).
* Additional stylesheet refactoring to help further reduce file size.
* Added new Pinterest Share Button Behavior option to Show Pinterest Images only.
* Fixed an issue where the Novashare JavaScript would not get enqueued properly if only using a shortcode on a URL.
* Fixed an SEO warning that was showing up in relation to the copy button link not being crawlable.
* Fixed a PHP error that could happen in a specific settings configuration.
* Added support for Social Warfare post meta to the Novashare Migrator.

= 1.3.5 - 12.01.2022 =
* Added new post meta option to add Pinterest Hidden Images.
* Updated a deprecated Yoast SEO open graph image filter.
* Added settings notice in Meta section to note if there is a compatible SEO plugin currently active.
* Fixed an issue with an invalid inline style printing for the Inline Content call to action.
* Fixed an issue in the block editor where certain Pin Images were overflowing their container.
* Added support for Grow Social attachment meta and Pinterest hidden images to the Novashare Migrator.

= 1.3.4 - 09.23.2022 =
* Added new Inline Content option to Show in Feeds.
* Added new novashare_inline filter.
* Added new novashare_floating filter.
* Added new novashare_short_link_url filter.
* Added support for {{network}} variable to all UTM parameter fields.
* Fixed an issue where inline shortcode was not printing if global post type was not selected.
* Fixed a PHP warning being generated in certain instances when global $post data was not available.
* Increased site limit in dropdowns on network settings page.

= 1.3.3 - 08.10.2022 = 
* Added new Follow Buttons Block, which allows you to quickly add and customize follow buttons for your social network profiles anywhere on your site (via the Block Editor, Customizer, or Widgets screen).
* Increased popup window size for LinkedIn for better usability.

= 1.3.2 - 06.30.2022 = 
* Added new novashare_pin_button_text filter.
* Added new novashare_total_share_count_text_plural and novashare_total_share_count_text_singular filters.
* Added new novashare_follow_network_link filter.
* Added new novashare_inline_excluded_filters filter.
* Added compatibility with SEOPress when using our open graph tags.
* Added fallback to featured image when using open graph and no post-specific meta image is set.
* Fixed an issue that was causing the Disable Pinning toggle on image blocks to be switched on by default in some cases.
* Fixed an issue where the default meta image would be prioritized over the featured image in open graph if no other meta details were set.
* Made an adjustment to popup window dimensions triggered by Pinterest image pins.
* Added filter integration with Perfmatters for better compatibility with Remove Unused CSS feature when running both plugins.
* Updated EDD plugin updater class to version 1.9.2.
* Translation file updates.

= 1.3.1 - 05.02.2022 =
* Added new Inverse on Hover design option for Inline Content and Floating Bar share buttons.
* Changed toggle CSS selectors to be more specific to prevent conflicts.
* Moved plugin settings header output to in_admin_header action hook for compatibility.
* Minor style adjustments to the new plugin UI.
* Added support for Grow Social share counts and post meta data to the Novashare Migrator.

= 1.3.0 - 03.30.2022 =
* Updated network admin settings page with UI improvements and support page.

= 1.2.9 - 03.29.2022 =
* Updated plugin settings UI.
* Added new novashare_bitly_link_generated action.
* Fixed an issue where the share window call to action background setting was not displaying correctly.
* Fixed an issue where the background color was not able to be changed for the click to tweet block in the block editor.
* Changed settings export file name date format to be easier to organize when managing multiples.
* Moved restore default functionality to a separate option on the tools page.
* Code refactoring.

= 1.2.8 - 02.24.2022 =
* Added new option to set a Default Social Image.
* Added new Subscribe Button along with a Subscribe Link field.
* Added prompt to display a confirmation dialog after clicking the copy button.
* Updates to TinyMCE code to prevent an error from occurring if localized script data is not available.
* Fixed an undefined index warning coming from settings.php.
* Minor plugin settings UI improvements.
* Refactored main JS file to be more efficient (25% smaller).

= 1.2.7 - 02.03.2022 =
* Added new Pin Image field to the Novashare section of the core image block editor.
* Added new hidden image functionality to the post meta Pinterest Image when share button is set to Show All Pinnable Images.

= 1.2.6 - 12.22.2021 =
* Added new Share Button feature.
* Added some extra logic to the floating bar on mobile that will push it past the footer when scrolling to the very bottom of the page.
* Added clarification to the tooltip for the floating bar top offset option to more clearly explain accepted values.
* Fixed a validation issue with the Pinterest image hover button HTML.

= 1.2.5 - 11.09.2021 =
* Improved reliability of Facebook share count requests due to API changes.
* Fixed an issue where the refresh share counts button was not working correctly in some configurations.
* Added plugin logo to WordPress plugin updates section.

= 1.2.4 - 11.05.2021 =
* Added support for new click to tweet accent color and default toggle states to shortcode builder.
* Fixed an issue where certain network links were not set to the correct protocol.
* Updated EDD plugin updater class to version 1.9.1.

= 1.2.3 - 11.02.2021 =
* Added new accent color options for click to tweet elements.
* Added three new default state toggles for click to tweet element options.
* Updated settings migration functions for easier compatibility with multisite.
* Code refactoring and cleanup.
* Fixed an issue where button links weren't working correctly on single attachment posts.
* Fixed undefined index warning in widget.php.
* Fixed an issue with the clean uninstall function.

= 1.2.2 - 09.24.2021 =
* Added Discord network support for Follow Buttons.
* Added Goodreads network support for Follow Buttons.
* Fixed an issue where HTML tags were getting included in the title when sharing an archive post.
* Updated post type selection options to include attachment posts.
* Added new novashare_permalink filter and available integration with AffiliateWP.
* Made some changes to our plugin updater function that should help with auto-updates in a multisite environment.
* Updated EDD plugin updater class to version 1.9.0.

= 1.2.1 - 09.02.2021 =
* Added new Show on Scroll options to Floating Bar.
* Added new novashare_button_attributes filter.
* Added new novashare_button_networks filter.
* Added new novashare_inline_position filter.
* Added new novashare_opengraph_meta_tags filter.
* Added some compatibility styles to Pinterest hover buttons to help with CLS in certain instances.

= 1.2.0 - 07.27.2021 =
* Added new Pinterest Share Button Behavior and an option to display a gallery of images by default.
* Added new Pinterest image pin options to change Button Position, Button Shape, and Hide Button Labels.
* Added new novashare_network_link filter.
* Added new novashare_inline_cta filter.
* Added new novashare_networks filter.
* Added new novashare_pinterest_image_excluded filter.
* Added support for our new Novashare Migrator tool.
* Improved reliability of Facebook share count requests due to API changes.
* Plugin UI navigation performance improvements.
* Fixed some compatibility issues with the follow widget and WordPress 5.8.
* Fixed an issue that was causing some one-per-line text fields to not save correctly.

= 1.1.9 - 06.18.2021 =
* Added new Excluded Images field to Pinterest options to exclude specific images based on their attribute string. Added new novashare_pinterest_image_excluded_attributes to go along with that option.
* Added new Twitter Count Service option with the ability to switch between TwitCount and OpenShareCount.
* Fixed LinkedIn share button link on mobile devices with the app installed.
* Removed value requirement for data-pin-nopin attribute.
* Made adjustments to the Novashare row links on the plugins page.
* Removed license activation check and corresponding links from the plugins page to improve back-end performance.
* Added readme.txt file.

= 1.1.8 – 05.11.2021 =
* Added new Top Offset option to Floating Bar.
* Added new Custom CSS box which will only print when Novashare is loaded.
* Added new post meta option to Disable Image Pins on an individual post.
* Added new Copy button to Inline Content and Floating Bar.
* Added expiration date to license tab.
* Updated AIOSEO functions to their latest filters for compatibility with Novashare meta details.
* Fixed an issue with Click to Tweet font styling on sites with dark backgrounds.
* Added support for data-pin-description attributes already present on images when using Pinterest hover buttons.
* Fixed an issue where Pinterest hover buttons were being applied to images even if the source had no valid extension.
* Fixed multiple PHP warnings coming from oembed functions in meta.php.

= 1.1.7 – 03.29.2021 =
* Added new Inline Content options for Call to Action.
* Added new Floating Bar mobile options for Background Padding, Fill Available Space, and Hide Total Share Count.
* Added new Floating Bar option for Container Offset.
* Added new Button Margin options for both Inline Content and Floating Bar.
* Added LINE network support for Follow Widget.
* General styling fixes and optimizations to improve performance when printing multiple button groups on the same page.
* Added support for novashare_mobile_networks filter to Follow Widget.
* Fixed an issue that was causing styles not to print properly when using a nested content shortcode on the page.
* Removed options for Remove Spacing which has been replaced with new Button Margin inputs.

= 1.1.6 – 02.11.2021 =
* Added new novashare_follow shortcode to print follow buttons.
* Added new novashare_floating shortcode to relocate floating bar output.
* Added new Floating Bar option to Show on Homepage.
* Added new Configuration option to Hide Meta Box in the WordPress editor.
* Added new Configuration option to enqueue Global Styles when using shortcodes or widgets on custom templates.
* Added new Messenger desktop link format if a Facebook App ID is available.
* Added a minimum image dimension check for Pinterest image hover buttons along with a new novashare_pinterest_image_minimum_dimension filter.
* Fixed an issue where the Click to Tweet menu button wasn’t showing in the Classic Editor.
* Fixed an AMP validation warning on the Pinterest image hover buttons.

= 1.1.5 – 01.20.2021 =
* Added compatibility with All in One SEO when using our open graph tags.
* Fixed an issue where button styles were not loading correctly when previewing a post.
* Fixed an issue where certain styles were not loading correctly when viewing an AMP post.
* Fixed a PHP warning related to combining HTTP + HTTPS share counts.
* Fixed an issue where Bitly URLs were being generated for LinkedIn.
* Updated Pinterest Image Hover button link to HTTPS.
* PHP 8 compatibility testing.
* Various code optimization.

= 1.1.4 – 12.21.2020 =
* Added new floating bar options to Show on Posts Page (blog feed or homepage) and Show on Archives.
* Added desktop link variations for the few networks that were previously only available on mobile. All networks will now show on both by default.
* Added Pinterest popup grid selection as a fallback if no specific image is set for the page.
* Added novashare_post_permalink filter to any instances where we get the permalink by post ID.
* Made some adjustments to our Pinterest image hover button container to prevent it from interfering with parent block elements.
* Updated EDD plugin updater class which will now allow for WordPress auto-update support.
* Organization improvements to plugin settings pages.

= 1.1.3 – 11.09.2020 =
* Added LINE, Messenger, and TikTok networks.
* Performance optimizations to the short link request function.
* Moved a small number of networks to only display on mobile devices. This list can be modified via our new novashare_mobile_networks filter.
* Added new novashare_ctt_tweet filter.
* Adjusted Open Graph title and description meta tags to remove line breaks and various other unwanted characters.
* Fixed an issue that was causing Open Graph meta tags to display on non-singular posts where Novashare is not displayed.
* Pinterest Image Hover Button adjustments for better compatibility.
* Added aria-label attributes to all network buttons for accessibility.
* Updated LinkedIn share link URL format.
* Added function to remove rows associated with a post from the novashare_meta table when that post is deleted.
* Fixed an issue with the Click to Tweet button not showing up in the Classic Editor.

= 1.1.2 – 11.02.2020 =
* Fixed a bug that was causing duplicate short link rows to be created in the novashare_meta table for some posts. These will automatically clear out over time, but you can also use our Purge Short Links option to immediately clear out all short link data.

= 1.1.1 – 10.09.2020= 
* Fixed an issue where certain custom styles were not displaying correctly when custom button colors were also set.

= 1.1.0 – 10.08.2020 =
* Added new Button Style options with 6 available styles for inline content and 2 available styles for the floating bar.
* Added new Button Layout option for inline content buttons with support for up to 6 columns.
* Added new Button Label options for inline content buttons to display social network labels next to their respective icons.
* Added new Total Share Count options for inline content and floating bar for positioning before and after social buttons as well as changing text color.
* Added new Remove Spacing options for inline content and floating bar to hide margins around buttons in either location.
* Added new Mobile Background Color for the floating bar.
* Multiple additions and improvements to JavaScript translation support throughout the plugin.
* Added top margin to inline content buttons displayed below post content.
* Added default variable to embed title filter for better error handling.
* Made small style adjustment to Pinterest image hover buttons for better compatibility with captions.
* Fixed multiple PHP warnings coming from the settings and main functions files.

= 1.0.9 – 08.31.2020 =
* Added new Social Follow Widget which allows you to add follow buttons for your social network profiles.
* Styling adjustments to the Pinterest image hover buttons for better compatibility.
* Added excerpt filter exclusion to prevent share button HTML from interfering with some excerpt snippets.
* Migrated to minified versions of our front-end JS and CSS files for increased performance for some sites.

= 1.0.8 – 07.28.2020 =
* Added Hacker News social network share button.
* Added SMS share button.
* Added new Button Alignment option to both Inline Content and Floating Bar settings.
* Added ‘novashare_meta_title’ filter to all places where a meta title is determined and returned for social links, open graph, etc…
* Made some adjustments to the content filter for Pinterest image hover buttons to prevent pins from being added to images outside of the loop.
* Front-end stylesheet compatibility improvements for Pinterest image hover buttons and mobile floating bar.
* AMP compatibility fixes.
* Thanks to the team at Kinsta for sharing a few bugs that are now fixed!

= 1.0.7 – 07.06.2020 =
* Added a share count recovery improvement to flag the recovery API calls to run again with the share count updater if there was a failed response returned from one of the networks the first time.
* Adjusted a tooltip translation that had an HTML tag in the translation string.
* Made some small improvements to novashare.js.
* Fixed an issue where the Click to Tweet shortcode was attempting to run outside of the content hook which was causing the inline styles to not print correctly.
* Added some additional logic to the Click to Tweet functions to strip HTML tags from the tweet shared in the URL.

= 1.0.6 – 07.02.2020 =
* Added new Share Count Recovery section including options to Combine HTTP & HTTPS URLs, Recover Previous Permalink Structure, Domain, & Post URLs.
* Added some additional logic to the Pinterest Hover image thumbnail filter to prevent hover buttons from appearing on images outside of the loop.
* Removed the error message that displayed if our inline shortcode was included on a page that did not have Novashare enabled.
* Fixed a styling bug in our plugin settings that was causing long option titles to interfere with the tooltip hover icons.

= 1.0.5 – 06.11.2020 =
* Added new Options section for Pinterest in plugin settings along with a new option to Enable Image Pins.
* Added some additional logic to novashare_is_post_allowed function to prevent post meta details from being queried if they are not needed.
* Added nofollow, noopener, and noreferrer attributes to all social share links elements.
* Changed WhatsApp link format to better support both desktop and mobile devices.
* Fixed a bug where the Call to Action text and position fields were not being populated automatically when inserting a Click to Tweet shortcode.
* Fixed a bug where the short link function was being triggered if certain conditions were met in the Block Editor.

= 1.0.4 – 05.28.2020 =
* Added new Floating Bar option to set the Mobile Max Width which will allow you to only show the floating bar’s mobile view below a certain width.
* Made some adjustments to the share button styles for better compatibility.
* Added exclusion attribute on Pinterest share button to prevent issues when their pinit.js script is also loaded.
* Updated tooltip link for the Twitter Username option.

= 1.0.3 – 05.20.2020 =
* Added new Configuration option to adjust the Share Counts Refresh Rate, along with a filter to pass in a custom set of refresh rates.
* Reworked front-end novashare.js file to not require jQuery. (Props to Andy Feliciotti for the suggestion)
* Added a new Novashare Inline Content shortcode for displaying inline content share buttons.
* Added an additional Inline Content Button Position option, “Don’t Add to Content”.
* Adjusted the Refresh Share Counts function to purge existing share counts before updating for the requested post.
* Fixed an issue where a row for Novashare meta details would sometimes be created before any data had been entered.

= 1.0.2 – 05.08.2020 =
* Various Multisite fixes and compatibility improvements.
* Fixed the label on Call to Action Position in the Click to Tweet shortcode popup.

= 1.0.1 – 05.03.2020 =
* Fixed a bug that was causing the stylesheet not to load correctly in certain cases if share counts were disabled.

= 1.0.0 – 05.01.2020 =
* Official launch version of Novashare!
* Fixed some styling issues on the network specific settings page.
* Fixed an issue where the Restore Defaults button wasn’t working on the main options tab.
* Added base translation files.
* Removed various old comments, cleaned up some code that was no longer being used.

= 0.1.0 =
* Added character limits to various text fields across plugin settings.
* Removed Pinterest Description from the Novashare Details post meta box.
* Updated EDD Updater Class to the latest version (1.7).
* Added additional checks to prevent the share updater function from running in places where it doesn’t need to.
* Fixed an issue where the Pinterest share button was not successfully grabbing the image URL for the link.
* Adjusted notifications for button trigger options.
* Added new options to Import and Export plugin settings in the Tools tab.
* Migrated Extras tab to new Tools tab.
* Fixed an issue where social share counts were still attempting to calculate on preview URLs.

= 0.0.9 =
* Added tooltip text and documentation links to the majority of plugin options.
* Added basic input prevention for invalid characters on various text inputs.
* Numerous styling changes and additions both on front end elements and in the plugin admin UI.

= 0.0.8 =
* Reworked the licensing tab user interface.
* Combined various network and licensing functions into a shared core set of functions.
* Fixed an issue with click to tweet boxes creating empty duplicates when surrounded by paragraph tags.
* Fixed an issue with total shares text display where there is only a single total share.
* Added credit to icon library sources in the main plugin file.
* Added breakpoint offset pixel for hiding above so the below and above options overlap correctly.
* Updated plugin description.

= 0.0.7 =
* Modified share count updater to save update timestamp even if no share counts are retrieved.
* Removed LinkedIn share counts.
* Finished integrating social button print functions with post meta display controls.
* Added UTM parameters to plugin settings page header links.

= 0.0.6 =
* Updated Facebook Graph API Calls to v6.0.
* Fixed various styling bugs.
* Added new configuration option to Purge Social Share Counts.
* Updated share counts refresh timer to check modified date instead of publish date.
* Updated admin enqueue function to only enqueue admin scripts and styles in necessary locations.

= 0.0.5 =
* User interface updates and improvements in the plugin settings and the front end styles.

= 0.0.4 =
* Fixed a bug that was preventing WordPress from automatically adding paragraph tags to content.
* Updated text domain in EDD Updater Class to match the rest of the plugin.

= 0.0.3 =
* Updated EDD Updater Class to the latest version (1.6.18).

= 0.0.2 =
* Updated meta box function to only display Novashare Details meta box on public post types.
* Updated Bitly functions to v4 of their API.

= 0.0.1 =
* First live version uploaded for testing.
