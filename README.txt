 === Sympose ===
Contributors: mklasen
Tags: conference, speakers, sponsors, schedule, sessions
Requires at least: 6.0
Tested up to: 6.6.1
Stable tag: trunk
Requires PHP: 5.6
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Sympose makes it easy for anyone to create a conference website. Install WordPress, install Sympose and kick start your conference. Sympose integrates with all WordPress themes.


== Description ==
Sympose is a WordPress plugin for conferences. Sympose makes it easy to create pages for conferences in WordPress. You can easily create schedules for events, and link the individual sessions to speakers and sponsors.


**Sympose Quick Start**

After activating Sympose, you can start shaping your event right away with the Quick Start!

=== Shortcodes ===

Below you'll find some Sympose shortcodes. You can also find specific shortcodes for your event in Sympose -> Shortcodes (in the WordPress dashboard)

= Shortcode example for displaying people =

`[sympose type="person" category="speakers" event="sympose" description="false" name="true"]`

This will display people from the category speakers and the event "sympose".

= Shortcode example for displaying a schedule =

`[sympose type="schedule" event="sympose"]`

This will display the schedule for the event "sympose".

= Shortcode example for displaying organisations =

`[sympose type="organisation" category="sponsors" event="sympose"]`

This will display organisations from the category sponsors and the event "sympose".

Check out other shortcodes (after creating posts and categories) in the Sympose -> Shortcodes menu.

== Installation ==

I recommend to install plugins via your WordPress Dashboard. Go to Plugins -> Add new, and search for `Sympose`.

== Screenshots ==

1. Example of schedule page
2. An example of a person/speaker profile page (with extensions)
3. An example of a session page (with extensions)
4. Sessions overview in dashboard
5. Sympose Quick Start
6. Sympose settings (with extensions)
7. Example of available shortcodes
8. Editing a person (with extensions)
9. Editing a session
10. Event taxonomy overview
11. Available extensions (Sympose -> Extensions)
12. An example of the people overview in the dashboard

== Extensions ==

Sympose is a free Wordpress plugin developed to manage events on your WordPress website. Sympose also provides a variety of extensions that add functionality to the main plugin.

== Changelog ==

= 1.4.8.5 =
* Fix bug in edit link

= 1.4.8.4 =
* Add classes in social media icons

= 1.4.8.3 =
* Remove support for Sympose Extensions
* General fixes and improvements
* Add support for placeholder images

= 1.4.8.2 =
* Bug fixes

= 1.4.8.1 =
* Disable extension check + Show events in tickets dashboard

= 1.4.8 =
* General fixes

= 1.4.7.9 =
* General fixes

= 1.4.7.8 =
* Add support for tracks in Sympose Shortcode

= 1.4.7.7 =
* Fixes issue in which other terms were also hidden when start date was in the past or non existen

= 1.4.7.5 =
* Make the people and organisations fields in person and organisation post types alphabetical.

= 1.4.7.4 =
* Only show valid ordered items when editing event
* Update the session datetimes, on save of a linked event, only when the event date changed.

= 1.4.7.3 =
* Add sympose_before_profile_image and sympose_after_profile_image actions

= 1.4.7.2 =
* Save selected people for organisation as ints. Solves an issue with people showing twice in widgets.

= 1.4.7.1 =
* Small bug fix

= 1.4.7 =
* Fixes issue in sample data generation.

= 1.4.6.5 =
* Sample data generation now imports sample logos.
* Allow customising the time column content in Dashboard.
* Only run actions for personal agenda when it's activated.
* Several small improvements.

= 1.4.6.4 =
* Improve the way the order of people and organisations are saved.

= 1.4.6.3 =
* Reformat output logic of list items like people or organisations.

= 1.4.6.2 =
* Add 'static' class to static session rows.
* Add option to show session participants after the session content.
* Define the sorting of people and organisations per event.

= 1.4.6.1 =
* Add filter for customising item links (sympose_customize_item_link)

= 1.4.6 =
* Fixes an issue where people were added to an organisation multiple times.

= 1.4.5 =
* Show draft, private and published sessions in the schedule when logged in.

= 1.4.4.1 =
* Small HTML Markup improvements

= 1.4.4 =
* Introduce sympose_before_schedule, sympose_before_schedule_event, sympose_after_schedule_event and sympose_after_schedule_event actions
* Introduce the sympose_session_row_dataset filter for adding extra information to a session row
* Fixes a bug where an image cannot be loaded
* Improve markup of the Sympose Session Information widget
* Add te sympose_information_widget_session_info_after action to the Sympose Session Information widget
* Introduce image sizes person-large and organisation-large
* Make the list of people in an organisation sortable and add an edit link
* When saving an organisation, sync the organisation to the person.
* When saving a person, sync the person to the organisation.
* Introduce "sympose_render_item_{$post->post_type}" and sympose_customize_person_short_description filter
* Introduce extra filters for the person and organisation post types in the dashboard.

= 1.4.1 - 1.4.3 =
* Several fixes

= 1.4.0 =
* Introduces personal agenda / agenda favorites
* Introduces block editor (Gutenberg) blocks
* Integrates the Sympose Session People and Sympose Session Organisations extensions into the main plugin
* Integrates the Sympose Session Profile and Sympose Session Profile extensions into the main plugin
* Integrates the Sympose Social Media plugin extension in the main plugin
* Allows event archive pages and automatically sets event for sympose schedule shortcode/block
* Prevent overriding sidebar on non single pages.
* Added hooks 'sympose_before_schedule_title' and 'sympose_after_schedule_title'

*Technical notes*
* Deployment to the WordPress repository is now done with Github actions.
* Reformatting

= 1.3.2 =
* Fixes the "No results found" issue when searching for sessions in the dashboard.
* Allows authors to use Sympose and adds extra filters for managing capabilities.
* Adds a missing parameter for register_rest_route which caused a notice to show.

= 1.3.1 =
* Add the option to show photo, name or photo and name on the schedule.
* Full code refactoring
* Published source code on https://github.com/conference7/sympose

= 1.3.0 =
* Combine all Sympose settings into one menu item in the WordPress Dashboard.

= 1.2.9 =
* Adds a filter that can change the schedule output of Sympose. (used by Sympose Extended Schedule and other plugins)
* Adds an option to mark a session as static session, disabling a link/read more link in the schedule.
* Adds missing tfoot element to schedule output.

= 1.2.8.1 =
* Minor bug fix: In some cases the person description was unintentionally added after every title.

= 1.2.8 =
* Include an image on the person/organisation overview in the dashboard.
* Fixes an error when a schedule is rendered for an event that does not exist.
* Adds people and organisations to the session overview in the dashboard.
* Make it possible to clear the attached people/organisations in Quick Start by selecting "Select.."

= 1.2.7 =
* Animate a scroll to top when error notices are generated in Quick Start
* Adds support for AM/PM times.
* Order the schedule based on post date, instead of session start date (session start dates are automatically set as post dates)


= 1.2.6 =
* Fixes a warning when the session information widget is shown, but no event is attached to the session
* Adds a settings link to the Sympose admin submenu, instead of showing 'Sympose'
* Correct the sessions link that shows after completing quick start
* Fixes an issue where sessions are marked future posts after editing via "Quick edit"
* Adds an option to replace the default sidebars with Sympose's sidebars
* When errors occur in Quick Start, make sure the notice is visible by automatically scrolling up.
* Collect the e-mail address from randomuser.me for Sympose Contact when generating sample data.
* Fixes an issue with the session order after generating data with Quick Start.


= 1.2.5 =
* Improves the setup wizard
* Extends Quick Start with the option to attach people/organisations to sessions
* Fixes a bug where a link to the event schedule was showing multiple times

= 1.2.4 =
* Introduces a setup wizard
* Integrates the quick start extension into Sympose core
* Adds responsive styling for schedule table
* Integrates CMB2 into Sympose core, instead of having to install it separately

= 1.2.3 =
* Fixes javascript bug for sortable lists

= 1.2.2 =
* Remove filter for number of extensions showing in Sympose -> Extensions
* Show active/installed extensions in Extensions dashboard *
* Fixed a wrong presentation of shortcodes *
* Add functionality for children sessions *
* Other small improvements *

= 1.2.1 =
* General Improvements
* Update session date/time when an event changes date.

= 1.2.0 =
* Code refactoring
* Sympose now follows WordPress Coding Standards

= 1.1.3 =
* Refreshes extensions on plugin activation
* General improvements

= 1.1.2 =
* Fixes issue with updating extensions on settings page

= 1.1.2 =
* Fixes a minor bug when creating sample data

= 1.1.1 =
* Call Flush Rewrite Rules on plugin activation
* Add labels for the Events taxonomy
* Extend the Create sample data function with a wider set of data

= 1.1.0 =
* Integrate remote extensions into Sympose Admin Menu
* Improve display of icons in Dashboard

= 1.0.10 =
* Move Page Schedule option to Current Session Plugin

= 1.0.9 =
* Extend Session Information widget with title input field

= 1.0.8 =
* Show the correct shortcodes in the WordPress Plugin Repository
* Fix an issue with session order

= 1.0.7 =
* Fix a bug in Settings Page

= 1.0.6 =
* Use normal image elements instead of div with backgrounds
* Optimize image sizes
* Improve error handling
* Correct shortcode examples

= 1.0.1 - 1.0.5 =
* Multiple small improvements

= 1.0.1 =
* Remove fontawesome and bad link to fontawesome stylesheet
* Change read-more class to sympose-read-more to avoid issues with themes
* Multiple small CSS improvements

= 1.0 =
* Initial version
