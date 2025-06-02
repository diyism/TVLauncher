    $ git clone https://github.com/diyism/TVLauncher
    
    $ curl -s "https://get.sdkman.io" | bash
    $ source "$HOME/.sdkman/bin/sdkman-init.sh"
    $ sdk install gradle
    
    $ cd TVLauncher/Main
    $ gradle wrapper --gradle-version 7.6
    $ ./gradlew assembleRelease
    $ ls -al app/build/outputs/apk/release/app-release-unsigned.apk
    $ jarsigner -verbose -sigalg SHA1withRSA -digestalg SHA1 -keystore ~/apk.keystore app/build/outputs/apk/release/app-release-unsigned.apk key-alias

# Android TV Launcher

## Screenshots
![Screen](Misc/1.png)
