# Firefox Custom Configuration Overview

This document outlines a custom Firefox configuration based on a set of policies. These policies control various browser settings to enhance privacy, user experience, and security. Below is a breakdown of the key configurations applied:

## General Policies

- **Block About Profiles**: Prevents access to about:profiles for managing profiles.
- **Default Download Directory**: Sets the default directory for downloaded files to `${home}/Downloads`.
- **Disable Firefox Accounts**: Disables the use of Firefox Accounts, preventing synchronization with the Firefox Cloud.
- **Disable Form History**: Disables saving form history in the browser.
- **Disable Master Password Creation**: Disables the option to set up a master password for Firefox's password manager.
- **Disable Profile Import & Refresh**: Disables the ability to import or refresh Firefox profiles.
- **Disable Telemetry**: Disables sending telemetry data to Mozilla for browser performance and usage analysis.
- **Display Bookmarks Toolbar**: Hides the bookmarks toolbar, setting it to "never" display.
- **Disable Pocket**: Disables the Pocket feature in Firefox, including any recommendations.
- **Hardware Acceleration**: Ensures that hardware acceleration is enabled for better performance.
- **No Default Bookmarks**: Disables the inclusion of default bookmarks when Firefox is first installed.
- **Offer To Save Logins**: Disables the prompt to save logins for websites.
- **Password Manager**: Completely disables the Firefox password manager feature.
- **Prompt for Download Location**: Always prompts the user to choose a location when downloading a file.
- **Show Home Button**: Displays the home button in the Firefox toolbar.
- **Translate Feature**: Disables Firefox's automatic translation feature.

## Cookie Policy

Only allows cookies from a predefined list of trusted websites:

- Google (Gmail, Classroom)
- GitHub (including Gist)
- DeepSeek (Chat)
- YouTube
- WhatsApp Web
- Figma
- ChatGPT

## User Messaging

- **Extension Recommendations**: Disables recommendations for extensions.
- **Feature Recommendations**: Disables feature recommendations from Firefox.
- **URL Bar Interventions**: Disables changes or interventions to the URL bar, such as search suggestions.
- **Skip Onboarding**: Skips the onboarding process when Firefox is first launched.
- **More from Mozilla**: Disables suggestions for other Mozilla products or services.
- **Firefox Labs**: Disables participation in Mozilla’s experimental features.

## Data Sanitization on Shutdown

On browser shutdown, the following data will be automatically sanitized:

- **Cache**
- **Cookies**
- **Browsing History**
- **Sessions**
- **Site Settings**

## Firefox Home Settings

- **Sponsored Top Sites**: Disables sponsored websites in the Firefox Home page.
- **Highlights**: Disables the display of highlights on the Firefox Home page.
- **Pocket**: Disables the Pocket service on the Firefox Home page.
- **Sponsored Pocket**: Disables sponsored content from Pocket.

## Extension Settings

- **uBlock Origin**: Forces the installation of uBlock Origin extension (version 1.42.0 or latest), directly from [this link](https://addons.mozilla.org/firefox/downloads/latest/ublock-origin/latest.xpi).

## Firefox Suggest

- **Sponsored Suggestions**: Disables sponsored suggestions in the address bar.

This configuration aims to provide a more streamlined and privacy-respecting browsing experience while disabling unnecessary features and recommendations.

## Installtion

- Download or copy the policies.json file.
- Place the file in the appropriate location on your system:
  - Linux: `/etc/firefox/policies/policies.json` or the equivalent directory for your Firefox configuration.
  - Windows: `C:\Program Files\Mozilla Firefox\distribution\policies.json`.
- Check out `about:policies` inside Firefox.

## Reference

- [Enforce policies on Firefox for Enterprise](https://support.mozilla.org/en-US/kb/enforcing-policies-firefox-enterprise)
- [Customize Firefox using policies.json](https://support.mozilla.org/en-US/kb/customizing-firefox-using-policiesjson)
