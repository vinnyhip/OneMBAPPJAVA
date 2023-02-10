# OneMBAPPJAVA
Min android app size in java language \
_Initial Size: 1411KB_

## Android min size app

Language: Java \
Release Size: 89 KB \
Installed Size: 283 KB\
Debug Size: 435 KB \

## Strategy: 
Remove LayoutConstraint \
Remove AppCompat \
App Gradle:
```groovy
buildTypes { 
  release { 
    minifyEnabled true 
    shrinkResources true 
    proguardFiles getDefaultProguardFile('proguard-android-optimize.txt'), 'proguard-rules.pro' 
  } 
}
```

After remove no used mipmap icons and adding the mipmap-nodpi the release size has changed to 61KB
