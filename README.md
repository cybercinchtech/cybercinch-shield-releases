# cybercinch-shield-releases

Public Maven repository hosting release artifacts for the CyberCinch Shield Android
SDK. No source code lives here — see `cybercinchtech/cybercinch-mobile-shield` for
that; this repo exists purely so `com.cybercinch:cybercinch-shield-android` can be
consumed as a normal Gradle dependency with no account or token required.

```kotlin
// settings.gradle.kts
dependencyResolutionManagement {
    repositories {
        google()
        mavenCentral()
        maven { url = uri("https://cybercinchtech.github.io/cybercinch-shield-releases/") }
    }
}
```

```kotlin
// app/build.gradle.kts
dependencies {
    implementation("com.cybercinch:cybercinch-shield-android:1.0.0")
}
```

Full integration docs: see the CyberCinch Shield Android SDK developer manual.
