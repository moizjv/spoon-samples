Sample android testing apks to run with spoon:
==============================================

This repository has sample apks for uiAutomator, espresso and android unit tests.

These apks have been built from [android-testing](https://github.com/googlesamples/android-testing) repository.

## Usage:

```
# to unlock
adb install unlock_apk-debug.apk
adb shell am start -n io.appium.unlock/.Unlock -a android.intent.action.MAIN -c android.intent.category.LAUNCHER -f 0x10200000
java -jar ./bin/spoon-runner-1.2.1-jar-with-dependencies.jar --apk espresso-sample/app-debug.apk --test-apk espresso-sample/app-debug-androidTest-unaligned.apk
```
