[android-components](../../index.md) / [mozilla.components.feature.share](../index.md) / [RecentAppsStorage](index.md) / [updateRecentApp](./update-recent-app.md)

# updateRecentApp

`fun updateRecentApp(selectedPackageName: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) [(source)](https://github.com/mozilla-mobile/android-components/blob/master/components/feature/share/src/main/java/mozilla/components/feature/share/RecentAppsStorage.kt#L31)

Increment the value stored in the database for the selected app. Then, apply a decay to all
other apps in the database. We do not need to handle overflow as it's not reasonably expected
to reach Double.MAX_VALUE for users

