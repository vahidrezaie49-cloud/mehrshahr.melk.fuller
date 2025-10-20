1. Generate keystore:
   keytool -genkey -v -keystore mehrshahrmelk.keystore -alias mehrshahr -keyalg RSA -keysize 2048 -validity 10000
2. base64 encode keystore:
   base64 mehrshahrmelk.keystore > keystore.b64
3. Create repo, push source, add secrets: KEYSTORE_BASE64, KEYSTORE_PASSWORD, KEY_ALIAS, KEY_PASSWORD
4. Trigger workflow or push to main. Download APK from Actions artifact.
