# OS Security and Privacy Monitoring App

This Android app helps users monitor and manage the permissions of other installed apps on their devices, increasing user awareness about potential privacy and security risks. It was developed for Android Pie (API 28).

## Features:

    Displays a list of installed apps on the user's device, categorized into system and other apps
    Provides detailed information about granted and denied permissions for each app
    Allows users to search and filter the app list for quick access to specific apps
    Clear search filters with a single tap to return to the full app list

Implementation

The app is developed using Android Studio and Kotlin. The app is tested on Android emulators to ensure performance across different Android devices.

## Classes:

AppListActivity

AppListActivity is responsible for displaying the list of installed apps on the user's device. The activity filters the apps into two categories: system apps and other apps. It also provides a search functionality to filter the app list based on the user's input. The search is implemented using a SearchView and ArrayAdapter.

LogActivity

LogActivity displays the permissions for a selected app and monitors the app's file access in the background. It retrieves the package name from the intent and sets up the back button to clear the app name. The activity creates a TextView for each permission and adds it to the layout. It also updates the UI to display the folder paths accessed by the app in a list view.

Util

Util is a utility class that contains helper methods for retrieving installed applications, system applications, and package information. It also provides methods for formatting dates and accessing shared preferences.

## Usage:

    Install the app on an Android device.
    Launch the app and view the list of installed apps, categorized into system and other apps.
    Select an app to see detailed information about its granted and denied permissions.
    Monitor the app's file access attempts and the accessed folder paths in real-time.
    Search for specific apps using the search functionality and clear the search filter with a single tap.

