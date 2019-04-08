# docker-androidsdk
Android SDK on Alpine

## Usage
An example of building a Cordova based Android project on this machine:

```bash
docker run -t -u root -v `pwd`:/workspace indiewebconsult/alpine-androidsdk /bin/bash -c \
  "cd workspace/platforms/android && ./gradlew cdvBuildDebug -Dorg.gradle.daemon=true -Pandroid.useDeprecatedNdk=true"
```
