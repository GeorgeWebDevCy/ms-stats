# MS Stats for Bridge Project

A WordPress plugin that adds a dedicated admin reporting dashboard with MasterStudy LMS statistics for the Bridge Project site.

**Requires:** MasterStudy LMS (free) — the plugin will not activate without it.

---

## Reports

| Tab                      | Description                                                       |
| ------------------------ | ----------------------------------------------------------------- |
| Overview                 | Total enrollments, enrolled users, active courses                 |
| Users by Country         | Enrolled users grouped by country (from MasterStudy profile)      |
| Enrollments by Language  | Enrollment count grouped by language code                         |
| Course Progress          | Avg progress %, fully completed count, completion rate per course |
| Quiz Completion          | Pass rate per course across all quiz attempts                     |
| Login Activity           | Active login session count per enrolled user                      |
| Certificates             | Certificates issued per course                                    |

---

## Requirements

- WordPress 5.8+
- PHP 7.4+
- [MasterStudy LMS](https://wordpress.org/plugins/masterstudy-lms-learning-management-system/) (free, must be active)

---

## Installation

1. Clone or download this repository into `/wp-content/plugins/ms-stats-for-bridge-project/`.
2. Run `composer install` inside the plugin folder (if vendor/ is not present).
3. Ensure **MasterStudy LMS** is installed and active.
4. Activate the plugin from the WordPress Plugins screen.
5. Go to **MS Stats** in the admin sidebar.

---

## Auto-Updates

This plugin uses [YahnisElsts/plugin-update-checker](https://github.com/YahnisElsts/plugin-update-checker) to pull updates directly from this GitHub repository. Bump the `Version:` header in the main plugin file and push to `main` — WordPress will surface the update automatically.

---

## Changelog

### 1.3.0

- Updated README files with accurate information.

### 1.2.0

- Added admin reporting dashboard with 7 tabbed reports.

### 1.1.0

- Added MasterStudy LMS dependency check (activation blocked without it).
- Added runtime admin notice if MasterStudy LMS is deactivated after install.
- Added GitHub auto-update mechanism via plugin-update-checker v5.6.

### 1.0.0

- Initial release.

---

## License

GPLv2 or later — see [LICENSE](http://www.gnu.org/licenses/gpl-2.0.html).
