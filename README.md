# Logger
## log封装

### 使用方法

module 下添加

    buildTypes {
        debug {
            buildConfigField "boolean", "LOG_DEBUG", "true"
        }
        release {
            buildConfigField "boolean", "LOG_DEBUG", "false"
        }
    }

     compile 'com.github.love-yanyi:Logger:1.0.1'
     或者
     compile 'com.yanyi.benyanyi:loglib:0.0.1'

     可设置是否打印JLog.init(boolean),默认不打印

<br/>

使用第一种引用则需project 下添加

    allprojects {
        repositories {
            jcenter()
            maven {
                url 'https://jitpack.io'
            }
        }
    }
    