# repo

#### Setting
```build.gradle
buildscript {
    ext.kotlin_version = "1.4.10"
    repositories {
        maven {
            url "https://raw.githubusercontent.com/eqgis/repo/main"
            //or url "https://repo.eqgis.cn"
        }
        google()
        jcenter()
    }
    dependencies {
        classpath 'com.android.tools.build:gradle:4.1.2'
        classpath "org.jetbrains.kotlin:kotlin-gradle-plugin:$kotlin_version"
    }
}

allprojects {
    repositories {

        google()
        jcenter()
        maven {
            url "https://raw.githubusercontent.com/eqgis/repo/main"
            //or url "https://repo.eqgis.cn"
        }
    }
}

```

```build.gradle
...
dependencies {
    //...
    implementation 'com.eqgis:eqtool:1.3.1'
    implementation 'com.eqgis:sceneform-sm:2.0.1'
}
...
```
