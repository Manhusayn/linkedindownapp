# LinkedIn Media Downloader — Android

A phone-first Android project intended for the OnePlus 9 5G.

## What it does

- Opens LinkedIn inside an Android WebView.
- Accepts LinkedIn URLs from the Android Share menu.
- Accepts pasted LinkedIn URLs.
- Uses Android DownloadManager for download URLs exposed by the page.
- Saves downloads to the public Downloads directory.
- Builds an ARM64-only release APK (`arm64-v8a`).

## Important limitation

LinkedIn may protect media behind authentication, dynamic requests, access controls,
or content delivery mechanisms that do not expose a normal downloadable URL.
This app does not bypass those controls. It can download media when LinkedIn exposes
a downloadable resource to the authenticated WebView/session.

## Build

The included GitHub Actions workflow builds the APK automatically on GitHub's runner.
No Android Studio is required on the user's phone.

Artifact:
`LinkedInMediaDownloader-arm64`
