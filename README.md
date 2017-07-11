# fleksy-emojis.json-updating

patching the Fleksy keyboard with support for new emojis

Fleksy was [acquired by Pinterest](http://fleksy.com/fleksy-acquired-by-pinterest/) on June 15, 2016 and ceased development. Unfortunately, the Android app was never open-sourced, and in the meantime, Android OS updates have brought new emojis to the table&mdash;emojis that can't be typed with the last released APK. This serves as a guide to keeping Fleksy emojis up to date, at least until the targeted APIs no longer are compatible with the current Android version.

This has been tested with Nougat emojis.

## Getting Started

All you need to do is update the APK file with the new ``emojis.json`` file. In the APK, this is stored in ``assets/emojis.json``. You can simply open the APK as an archive.

Then run the following to resign the APK.

```bash
./bin/signapk.sh com.syntellia.fleksy.keyboard_8.3.2.apk <keystore_file> <keystore_password> <alias>
```

You can generate a keystore by

```bash
keytool -genkeypair -v -keystore <keystore_file> -alias <alias> -keyalg RSA -keysize 2048 -validity 10000
```
