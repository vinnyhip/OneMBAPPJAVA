# OneMBAPPJAVA
Min android app size in java language \
_Initial Size: 1411KB_

## Android min size app

Language: Java

### Release Size: 21,0 KB
![image](https://user-images.githubusercontent.com/975220/225172206-e157b712-0672-4381-901d-dba57e959580.png)

### Installed Size: 102 KB
![image](https://user-images.githubusercontent.com/975220/225172822-529ac32e-130a-454f-b78c-25e264546161.png)

### Debug Size: 37,4 KB
![image](https://user-images.githubusercontent.com/975220/225172385-b5f260db-dfb3-415a-80c1-bd49b9c979ed.png)


## Strategy: 
Remove all implementation dependencies

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
