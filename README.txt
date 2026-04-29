=== MS Stats for Bridge Project ===
Contributors: orionaselite
Donate link: https://www.georgenicolaou.me/
Tags: masterstudy, lms, stats, reports, bridge project
Requires at least: 5.8
Tested up to: 6.7
Requires PHP: 7.4
Stable tag: 1.3.0
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Admin dashboard with LMS statistics and reports for the Bridge Project — requires MasterStudy LMS.

== Description ==

MS Stats for Bridge Project adds a dedicated admin reporting dashboard that surfaces key MasterStudy LMS metrics for the Bridge Project site.

**Reports included:**

* **Overview** — Total enrollments, enrolled users, and number of active courses at a glance.
* **Users by Country** — Breakdown of enrolled users grouped by country (from MasterStudy profile data).
* **Enrollments by Language** — Total enrollments grouped by language code.
* **Course Progress** — Per-course average progress %, fully completed count, and completion rate with visual bar.
* **Quiz Completion** — Per-course quiz pass rate across all attempts, with a visual pass-rate bar.
* **Login Activity** — Count of active login sessions per enrolled user.
* **Certificates** — Number of certificates issued per course.

**Requirements:**

* MasterStudy LMS (free) must be installed and active. The plugin will not activate without it.

== Installation ==

1. Upload the `ms-stats-for-bridge-project` folder to the `/wp-content/plugins/` directory.
2. Ensure MasterStudy LMS is installed and active.
3. Activate the plugin through the **Plugins** menu in WordPress.
4. Navigate to **MS Stats** in the WordPress admin sidebar.

== Frequently Asked Questions ==

= Does this plugin work without MasterStudy LMS? =

No. The plugin will refuse to activate if MasterStudy LMS is not installed and active. A notice is displayed if MasterStudy LMS is deactivated after activation.

= Where does the country data come from? =

From the `masterstudy_personal_data` user meta field that MasterStudy LMS stores when users fill in their profile.

= Why does the Login Activity tab show "Active Sessions" instead of a full login history? =

WordPress does not natively log historical login counts. The count shown reflects the number of active/recent login sessions stored in the `session_tokens` user meta key.

== Screenshots ==

1. Overview tab — total enrollment statistics.
2. Course Progress tab — per-course completion rates.
3. Quiz Completion tab — pass rates per course.

== Changelog ==

= 1.3.0 =
* Updated README.txt and README.md with accurate plugin information.

= 1.2.0 =
* Added admin reporting dashboard with 7 tabbed reports.
* Overview, Users by Country, Enrollments by Language, Course Progress, Quiz Completion, Login Activity, Certificates.

= 1.1.0 =
* Added MasterStudy LMS dependency check on activation (wp_die if missing).
* Added runtime guard — shows admin notice if MasterStudy LMS is deactivated.
* Added GitHub-based auto-update mechanism via plugin-update-checker.

= 1.0.0 =
* Initial release.

== Upgrade Notice ==

= 1.3.0 =
README updates only. No functional changes.

= 1.2.0 =
Major update: admin reporting dashboard added. Upgrade to access LMS stats.

= 1.1.0 =
Adds MasterStudy LMS dependency enforcement and auto-update support.
