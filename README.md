# Uniqueway Android SDK

本sdk为了项目与项目之间解耦. 并且有很多东西可以复用.所以提出建立本项目. 

## 如何使用 ?

project build gradle

```
allprojects {
    repositories {
        jcenter()
        maven {
            url "http://jenkins.uniqueway.in:8081/nexus/content/repositories/uniqueway/"
        }
    }
}
```

module build gradle

```
 compile 'com.uniqueway:socialsdk:1.0.0'
 compile 'com.uniqueway:circleviewpagerindicator:1.0.0'
```

## 如何修改源码

- git clone http://git.uniqueway.in/uniqueway/AndroidSDK.git
- ./gradlew clean build
- 找到你要修改的源码,版本号加一,并且提交 `merge request`
- 打开gradle面板,找到 module->upload->uploadArchives.
- 控制台如果输出successful.就代表成功.
- 使用的时候.用你最新的版本号替代老版本.

