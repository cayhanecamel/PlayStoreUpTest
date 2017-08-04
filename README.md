PlayStoreUpTest
==============
gradle-play-publisherとfastlaneの両方に対応したプロジェクト

## gradle-play-publisherでのDeploy
```
Play Store tasks
----------------
bootstrapReleasePlayResources - Downloads the play store listing for the Release build. No download of image resources. See #18.
generateReleasePlayResources - Collects play store resources for the Release build
publishApkRelease - Uploads the APK for the Release build
publishListingRelease - Updates the play store listing for the Release build
publishRelease - Updates APK and play store listing for the Release build

```

↓で、apkをビルドして、apkと付属品を全て
```
./gradlew publishRelease
```

## fastlaneでのDeploy
```
fastlane supply deploy
```