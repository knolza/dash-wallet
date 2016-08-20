Welcome to _Dash Wallet_, a standalone Gamblr payment app for your Android device!

This project contains several sub-projects:

 * __wallet__:
     The Android app itself. This is probably what you're searching for.
 * __market__:
     App description and promo material for the Google Play app store.
 * __integration-android__:
     A tiny library for integrating Gamblr payments into your own Android app
     (e.g. donations, in-app purchases).
 * __sample-integration-android__:
     A minimal example app to demonstrate integration of digital payments into
     your Android app.

You can build all sub-projects at once using Gradle:

`gradle clean build`

ou can build all sub-projects at once using Gradle:

gradle clean build -x test

Full Guide for building the APK:
### build gamblrj

$ git clone https://github.com/knolza/gamblrj.git

$ cd gamblrj

$ git checkout gamblr-0.1

$ mvn clean install -DskipTests

### build java-wns-resolver

$ git clone https://github.com/knolza/java-wns-resolver.git

$ cd java-wns-resolver

$ git checkout gamblr-0.1

$ mvn clean install -DskipTests

### build Gambler-Wallet

$ cd ..

$ git clone https://github.com/knolza/gamblr-wallet.git

$ cd gamblr-wallet

$ git checkout gamblr-0.1

$ ./gradlew clean build -x test
