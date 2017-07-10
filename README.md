# fleksy-emoji.json-updating
patching the Fleksy keyboard with support for new emojis

## Getting Started

First install the APK

```bash
java -jar bin/apktool_2.2.3.jar if apk/com.syntellia.fleksy.keyboard_8.3.2-394_minAPI16\(armeabi\,armeabi-v7a\)\(nodpi\).apk
 ```

Then decompile the app

```bash
java -jar bin/apktool_2.2.3.jar d apk/com.syntellia.fleksy.keyboard_8.3.2-394_minAPI16\(armeabi\,armeabi-v7a\)\(nodpi\).apk
```

Then copy the emoji.json file

```bash
cp assets/emojis.json com.syntellia.fleksy.keyboard_8.3.2-394_minAPI16\(armeabi\,armeabi-v7a\)\(nodpi\)/assets/emojis.json
```

And then recompile

```bash
java -jar bin/apktool_2.2.3.jar b com.syntellia.fleksy.keyboard_8.3.2-394_minAPI16\(armeabi\,armeabi-v7a\)\(nodpi\)/
```
