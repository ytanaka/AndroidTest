AndroidTest
===========

gradle setting
--------------

    $ cat ~/.gradle/gradle.properties
    
    RELEASE_STORE_FILE=~/android-release.keystore
    RELEASE_STORE_PASSWORD=*****
    RELEASE_KEY_ALIAS=*****
    RELEASE_KEY_PASSWORD=*****

keystore setting
----------------

    $ keytool -genkey -v -keystore xxxxx.keystore -alias xxxxx -keyalg RSA -validity 10000

build
-----

    $ ./gradlew assembleRelease
