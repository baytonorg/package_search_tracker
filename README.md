# PACKAGE SEARCH

**PACKAGE SEARCH** is a modern Android management tool designed to provide detailed insights into the apps installed on an Android device. With the ability to search, filter, and export app data, PACKAGE SEARCH aims to make Android app management simple, efficient, and accessible.

---

## Features

- **App Search & Filtering**: Easily search or scroll through your installed apps, and use advanced filtering options to refine results based on package name, version, install date, etc.
- **App Details**: View detailed information about each app, including version, target API, permissions, install source, and more.
- **Unavailable Apps**: Identify apps that are preloaded on your Android build but unavailable for the current user, possibly due to carrier restrictions or device management.
- **Export to CSV**: Export your app data, including installed and unavailable apps, to a CSV file for further analysis or sharing.
- **Support for Translations**: PACKAGE SEARCH is available in multiple languages, with a community-driven translation process.

---

## Contributing

The primary focus of this repository is for **issue tracking**. However, contributions related to translations are welcomed also.

### Issue Reporting
If you encounter a bug, or have a feature request, please create a new issue in this repository. Provide as much detail as possible, including:

- **Device Information** (Model, Android version, etc.)
- **Steps to Reproduce** (If applicable)
- **Expected Outcome** vs **Actual Outcome**
- Screenshots or logs (if relevant)

### Feature requests
If you'd like to see new or improved functionality, feel free to [vote on, or create](https://github.com/baytonorg/package_search_tracker/issues), an issue. Those already existing can be voted on (👍), otherwise templates exist outlining the information desired when raising an issue. Please use them!

### Translations
Translations are maintained under the following directory:

- [PACKAGE SEARCH Translations](https://github.com/baytonorg/package_search_tracker/tree/main/app/src/main/res)

If you’d like to contribute a new language or update an existing translation, please:

1. Fork the repository.
2. Navigate to (or create) the appropriate language folder.
3. Update the XML file (using the template below as a reference).
4. Submit a Pull Request (PR) to the repository for review.

#### Translation Template Example
Here’s a template you can follow when contributing. Be mindful of the comments, as there are restrictions on _some_ strings:

```xml
<?xml version="1.0" encoding="utf-8"?>
<resources>
    <!-- Titles and such -->
    <string name="app_name">PACKAGE SEARCH</string>
    <string name="app_launcher_name">PACKAGE SEARCH</string>
    <string name="app_topbar_title">Package Search</string>
    <string name="search_label">Search</string>
    <string name="intro_text">Search or scroll to locate your application, tap an app card for more details, or long-press the card to copy the package name. Apps with long package names can be scrolled horizontally.</string>

    <!-- Unavailable apps content -->
    <string name="unavailable_apps_title">Unavailable apps</string>
    <string name="unavailable_apps_text">The following applications are preloaded into this Android build, but are not made available for the current user. This may be due to a carrier-specific config (RRO), or because this device is under management.</string>
    <string name="unavailable_apps_learn_more">Learn more</string>
    <string name="unavailable_apps_learn_more_cont">about Android Enterprise &amp; vital apps.</string>

    <!-- Filter / sort - Used for the name of each "Sort by" option within the filter dialogue, as well as referenced in the main activity -->
    <string name="filter_option_title">Title</string>
    <string name="filter_option_pname">Package name</string>
    <string name="filter_option_idate">Install date</string>
    <string name="filter_option_utime">Last update</string>

    <!-- Filter popup -->
    <string name="filter_app_state_title">App state</string>
    <string name="filter_app_type_title">App type</string>
    <string name="sort_title">Sort by</string>
    <string name="close_popup">Close</string>

    <!-- Search function -->
    <!-- Filter options. These define how apps are filtered, e.g. min:23 -->
    <!-- also used throughout the application for logic. Any translation must be a one-word equivalent -->
    <string name="filter_name">name</string>
    <string name="filter_package">package</string>
    <string name="filter_version">version</string>
    <string name="filter_code">code</string>
    <string name="filter_target">target</string>
    <string name="filter_min">min</string>
    <string name="filter_profile">profile</string>
    <string name="filter_state">state</string>
    <string name="filter_type">type</string>
    <string name="filter_source">source</string>
    <string name="filter_state_enabled">enabled</string>
    <string name="filter_state_disabled">disabled</string>
    <string name="filter_state_unavailable">unavailable</string>
    <string name="filter_type_user">user</string>
    <string name="filter_type_system">system</string>
    <string name="filter_type_other">other</string>

    <!-- App states & status -->
    <string name="app_state_enabled">Enabled</string>
    <string name="app_state_disabled">Disabled</string>
    <string name="app_state_unavailable">Unavailable</string>
    <string name="app_type_user">User</string>
    <string name="app_type_system">System</string>
    <string name="app_type_other_profiles">other users</string>

    <!-- Not found & messages -->
    <string name="not_found">No applications found matching your search or chosen filter. Try again or check the spelling?</string>
    <string name="no_more_results">There are no more results</string>

    <!-- Toasts -->
    <string name="toast_no_browser">No browser available</string>
    <string name="toast_pname_copied">Package name copied to clipboard</string>
    <string name="toast_unavailable_no_info">Unavailable apps report no information</string>
    <string name="toast_export_failed">Failed to export data</string>
    <string name="toast_no_app_available">No application available</string>
    <string name="toast_app_no_can_launch">App doesn\'t support launching</string>
    <string name="toast_failed_download_data">Failed to export app data</string>

    <!-- App details -->
    <string name="app_details_version_code">Version (code)</string>
    <string name="app_details_version">Version</string>
    <string name="app_details_code">Version code</string>
    <string name="app_details_installed">Installed</string>
    <string name="app_details_updated">Updated</string>
    <string name="app_details_undetermined">Undetermined</string>
    <string name="app_details_nodata">No data</string>
    <string name="app_details_target_version">Target Android version</string>
    <string name="app_details_minimum_version">Minimum Android version</string>
    <string name="app_details_other_users">Other user(s)</string>
    <string name="app_details_state">State</string>
    <string name="app_details_type">Type</string>
    <string name="app_details_source">Source</string>

    <string name="app_details_preloaded">Preloaded</string>
    <string name="app_details_preloaded_via_play">Preloaded, updated via Play</string>
    <string name="app_details_unknown_source">Unknown source</string>
    <string name="app_details_category_too_low">Android version too low to retrieve category</string>

    <string name="install_warning">System apps don\'t normally report an accurate date.</string>

    <string name="app_details_play_app_category">Play App Category</string>

    <string name="app_details_permissions_title">Permissions</string>
    <string name="app_details_permissions_granted">Granted</string>
    <string name="app_details_permissions_not_granted">Not granted</string>

    <string name="app_details_general_title">General information</string>
    <string name="app_details_manifest_title">Manifest</string>
    <string name="app_details_activities_title">Activities</string>
    <string name="app_details_services_title">Services</string>
    <string name="app_details_receivers_title">Receivers</string>
    <string name="app_details_providers_title">Providers</string>

    <string name="manifest_permissions_title">Manifest permissions</string>

    <string name="app_details_not_found">App details not found</string>
    <string name="app_details_no_permissions">No permissions declared.</string>
    <string name="app_details_no_info">No information found.</string>

    <string name="open_app_action">Open app</string>
    <string name="open_app_info_action">App info</string>
    <string name="open_google_play_action">Google Play</string>
    <string name="download_app_data_action">Export data</string>

    <!-- Alert dialogue -->
    <string name="alert_export_dialog_title">Export complete</string>
    <string name="alert_export_dialog_text">Do you want to open or share the file?</string>
    <string name="alert_action_open">Open</string>
    <string name="alert_action_share">Share</string>

    <string name="intent_package_updated">Package updated: %1$s</string>
    <string name="intent_package_added">Package added: %1$s</string>
    <string name="intent_package_changed">Package changed: %1$s</string>
    <string name="intent_package_removed">Package removed: %1$s</string>
    <string name="intent_package_action">Package action: %1$s for %2$s</string>

    <!-- Settings -->
    <string name="available_actions_title">Available actions</string>
    <string name="app_details_title">App details</string>

    <!-- Cards -->
    <string name="card_support_title">Get support</string>
    <string name="card_support_text">Visit the project page for help.</string>

    <string name="card_discord_title">Join Discord</string>
    <string name="card_discord_text">Join the BAYTON discord for help &amp; advice.</string>

    <string name="card_feedback_title">Send feedback</string>
    <string name="card_feedback_text">This will open a browser window, if permitted.</string>

    <string name="card_export_title">Export all apps to CSV</string>
    <string name="card_export_text">Save or share a file containing all applications.</string>

    <!-- BAYTON branding -->
    <string name="about_package_search">PACKAGE SEARCH is a modern Android management project from bayton.org. For available actions and application support, please tap settings in the top right corner.</string>

    <!-- Generic -->
    <string name="yes">Yes</string>
    <string name="no">No</string>
    <string name="unknown">Unknown</string>

</resources>
```
Android follows the **BCP 47** standard for naming language and region codes when defining different string resources in an app. Each language or locale gets its own folder under the `res` directory, and the folder name is structured based on the language and sometimes the region or script. 

The general format for Android resource folders is:

```
res/values-<language>-<region>
```

##### Example folder names:

- **English (default)**: `res/values/strings.xml`
- **French**: `res/values-fr/strings.xml`
- **Spanish (Spain)**: `res/values-es/strings.xml`
- **Spanish (Mexico)**: `res/values-es-rMX/strings.xml`
- **Chinese (Simplified)**: `res/values-zh/strings.xml`
- **Chinese (Traditional, Taiwan)**: `res/values-zh-rTW/strings.xml`

##### Folder naming structure:

1. **Language code** (`<language>`): 
   - Two lowercase letters, e.g., `en` for English, `fr` for French.
   
2. **Region code** (`<region>`): 
   - Two uppercase letters following `r`, e.g., `rUS` for the United States, `rGB` for Great Britain, `rMX` for Mexico.
   
3. **Script code** (optional): 
   - For certain scripts, you may use a script code like `Latn` (Latin) or `Cyrl` (Cyrillic), e.g., `values-bn-Latn`.

##### Resource Folder Examples:

| Language           | Folder Name       | Description                              |
|--------------------|-------------------|------------------------------------------|
| Default (English)   | `values/`         | Default strings                          |
| English (US)        | `values-en-rUS/`  | English strings for the US               |
| French              | `values-fr/`      | French strings                           |
| German (Austria)    | `values-de-rAT/`  | German strings for Austria               |
| Chinese (Simplified)| `values-zh/`      | Chinese Simplified                       |
| Chinese (Taiwan)    | `values-zh-rTW/`  | Chinese Traditional for Taiwan           |
| Arabic              | `values-ar/`      | Arabic strings                           |

##### Resource on what to name the folders:

The [official Android documentation](https://developer.android.com/guide/topics/resources/localization) provides a complete guide for localization and the proper naming conventions for these folders. It explains how to structure `res/values` directories to target specific languages, regions, and even scripts.

Additionally, you can refer to the [IANA Language Subtag Registry](https://www.iana.org/assignments/language-subtag-registry/language-subtag-registry) to explore all the possible language, script, and region subtags available. 

### Pull Requests (PRs)
When submitting a PR for **code changes**, ensure you:

- Define the language the translation is for.
- Include clear commit messages.
- Ensure you’ve updated the correct language file.
- Ensure strings remain consistent with other translations (only the text changes, not the structure).

---

## When Will Translations Appear in the App?

Translations submitted via PR will be reviewed and merged into the codebase. Once merged, they will appear in the next release of PACKAGE SEARCH, which is updated periodically based on changes, bug fixes, and new features.

---

## Community and Support

- **Join Discord**: [Join the BAYTON Discord for help and advice](https://discord.gg/5yMfb9UWm9)
- **Project Page**: [PACKAGE SEARCH on bayton.org](https://bayton.org/projects/package-search)

For general questions or support, visit the project page or Discord community.
