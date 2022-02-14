# dart-labs

## Development

- https://flutter.dev/
- https://docs.flutter.dev/get-started/install/linux#install-flutter-using-snapd
- https://fossbytes.com/best-android-emulators-linux/

sudo apt install openjdk-17-jre-headless openjdk-17-jdk-headless 

    java -version
    javac -version
    which java
    echo \$JAVA_HOME

    ls /usr/lib/jvm
    ls /usr/lib/jvm/java-17-openjdk-amd64/bin

    cat /etc/environment

    echo \$(jrunscript -e 'java.lang.System.out.println(java.lang.System.getProperty("java.home"));')

    echo 'System.out.println(java.lang.System.getProperty("java.home"));' | jshell -

sudo snap install android-studio --classic

    echo '# Configure the ANDROID_HOME environment variable' >> ~/.bashrc
    echo 'export ANDROID_HOME="$HOME/Android/Sdk"' >> ~/.bashrc
    echo 'export PATH="$PATH:$ANDROID_HOME/emulator"' >> ~/.bashrc
    echo 'export PATH="$PATH:$ANDROID_HOME/tools"' >> ~/.bashrc
    echo 'export PATH="$PATH:$ANDROID_HOME/tools/bin"' >> ~/.bashrc
    echo 'export PATH="$PATH:\$ANDROID_HOME/platform-tools"' >> ~/.bashrc

    source ~/.bashrc # load the config into your current shell

    nano ~/.bashrc # check

    echo $ANDROID_HOME
    echo $PATH

sudo snap install androidsdk

    androidsdk --list

sudo snap install flutter --classic

    flutter sdk-path
    
    flutter doctor

    flutter emulators
    
sudo snap install anbox --beta --devmode

sudo apt install adb

  adb devices

  adb install AdobeReader-arm64-v8a-release.apk

sudo snap install scrcpy