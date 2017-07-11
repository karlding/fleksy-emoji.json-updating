# fleksy-emoji.json-updating

an attempt at patching the Fleksy keyboard with support for new emojis

## Getting Started

All you need to do is update the ZIP file with the new ``emoji.json``, then run

```bash
./signapk.sh com.syntellia.fleksy.keyboard_8.3.2.apk <keystore_file> <keystore_password> <alias>
```

You can generate a keystore by

```bash
keytool -genkeypair -v -keystore <keystore_file> -alias <alias> -keyalg RSA -keysize 2048 -validity 10000
```
