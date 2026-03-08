# Template React Native 724

A React Native 0.74 template project for quick setup and reference.

## How this template was created

```bash
npx @react-native-community/cli init TemplateReactNative74 --version 0.74 --package-name template.reactnative.v74
```

## Environment

| Tool       | Version  | Notes                                      |
| ---------- | -------- | ------------------------------------------ |
| Java       | 17       | Required for Android                        |
| Node       | 22       | Required for React Native                   |
| Gradle     | 8.6    | See `android/gradle/wrapper/gradle-wrapper.properties` |
| Ruby       | 3.2.2    | Used by CocoaPods scripts                   |
| macOS      | 26.3     | Development host                            |
| CocoaPods  | 1.16.2   | iOS dependency manager                      |
| Xcode      | 26.0.1   | iOS development                             |

## Check versions

| Command               | Purpose                              |
| --------------------- | ------------------------------------ |
| `java -version`       | Installed Java version               |
| `node -v`             | Installed Node.js version            |
| `ruby -v`             | Installed Ruby version               |
| `xcodebuild -version` | Xcode version and build number       |
| `pod --version`       | CocoaPods version                    |
| `sw_vers`             | macOS version (`sw_vers -productVersion` for version only) |

```bash
java -version
node -v
ruby -v
xcodebuild -version
pod --version
sw_vers
```

## Switch versions (macOS)

```bash
export JAVA_HOME=$(/usr/libexec/java_home -v 17)
nvm use 22
nvm alias default 22
```

## Install dependencies

```bash
npm install
cd ios && pod install && cd ..
```

## Run the project

- **Android:** `npm run android`
- **iOS:** `npm run ios`
- **iOS (specific simulator):** `npm run ios -- --simulator "iPhone 17"`
