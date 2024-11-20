# android
Android development knowledge

Prepare Dev Env
```
C:\jdk-21.0.5+11\
https://developer.android.com/studio#command-tools
sdkmanager "platforms;android-29" "ndk;25.2.9519653"

Env Variable:
ANDROID_HOME=C:\Android\sdk
JAVA_HOME=C:\jdk-21.0.5+11
PATH=%JAVA_HOME%\bin, C:\Android\sdk\cmdline-tools\latest\bin
```
Build APK
```
$ go install golang.org/x/mobile/cmd/gomobile@latest
$ gomobile init

mkdir go-mobile-basic2
cd go-mobile-basic2
go mod init go-mobile-basic2
go get golang.org/x/mobile/example/basic
gomobile build -androidapi 19 golang.org/x/mobile/example/basic
gomobile install -androidapi 19 golang.org/x/mobile/example/basic
```
