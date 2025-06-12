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

https://github.com/baytonorg/package_search_tracker/blob/main/app/src/main/res/values/strings.xml

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
