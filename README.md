# OneMBAPPJAVA
Min android app size in java language

Initial Size: 1411KB

Android min size app

Language: Java 
Release Size: 89 KB Debug Size: 435 KB

Strategy Remove LayoutConstraint Remove AppCompat App Gradle buildTypes { release { minifyEnabled true shrinkResources true proguardFiles getDefaultProguardFile('proguard-android-optimize.txt'), 'proguard-rules.pro' } }

Build Gradle
