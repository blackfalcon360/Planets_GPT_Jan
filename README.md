# PlanetCompass

Live planet-position compass for Android.

## Features
- Phone compass / rotation sensor
- GPS observer location
- Approximate live azimuth and altitude for Mercury, Venus, Mars, Jupiter, Saturn, Uranus and Neptune
- Jetpack Compose UI
- GitHub Actions debug APK build

## GitHub Actions
The workflow is `.github/workflows/build.yml`.

It uses JDK 17 and Gradle 8.7, then runs:

`gradle assembleDebug --no-daemon`

The generated APK is renamed to `PlanetCompass.apk` and uploaded as a GitHub Actions artifact.

## Accuracy
The planetary engine uses simplified orbital elements for general sky orientation and education. It is not intended for precision telescope pointing.
