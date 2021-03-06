# Integration Guide \(Lite\)

## **Steps to integrate Acquire android-sdk-lite are as follows :**

**Step 1 :**

Add the SDK to your project by including the following snippets in the **`build.gradle`** file:

Project level build.gradle :

```javascript
allprojects {
...
    repositories {
   // Add this lines 
        maven {
                url "https://android-sdk.acquire.io/artifactory/libs-release-local/"
        }
    }
...
}

```

Module build.gradle :

```javascript
dependencies {
    implementation 'com.acquireio:lite:3.+'
    implementation "org.jetbrains.kotlin:kotlin-stdlib-jdk7:1.4.10"
    implementation("org.jetbrains.kotlin:kotlin-reflect:1.4.20")
    implementation 'androidx.appcompat:appcompat:1.2.0'
    implementation 'com.google.android.material:material:1.2.1'
    implementation 'androidx.core:core-ktx:1.3.1'
    implementation 'androidx.constraintlayout:constraintlayout:2.0.4'
    implementation "org.jetbrains.kotlinx:kotlinx-coroutines-core:1.3.9"
    implementation "org.jetbrains.kotlinx:kotlinx-coroutines-android:1.3.9"
    implementation 'com.squareup.okhttp3:okhttp:4.8.1'
    implementation ('io.socket:socket.io-client:1.0.0') {
        exclude group: 'org.json', module: 'json'
    }
    implementation 'com.google.code.gson:gson:2.8.6'
    implementation 'androidx.lifecycle:lifecycle-extensions:2.2.0'
    implementation "androidx.fragment:fragment-ktx:1.2.5"
    implementation "androidx.room:room-runtime:2.2.5"
    kapt "androidx.room:room-compiler:2.2.5"
    implementation "androidx.room:room-ktx:2.2.5"
    implementation 'org.greenrobot:eventbus:3.2.0'
    implementation 'com.squareup.picasso:picasso:2.71828'
    implementation 'androidx.emoji:emoji-appcompat:1.1.0'
    implementation 'pl.droidsonroids.gif:android-gif-drawable:1.2.20'
    implementation 'androidx.browser:browser:1.2.0'
}
```

**Step 2 :**

Initialize Acquire in the **`onCreate()`** method of an Activity where you plan to use the SDK, or an Application subclass. Use the initialization details provided by the Acquire Support admin and an Application instance:

```javascript
class XYZApp : Application() {
    override fun onCreate() {
        super.onCreate()
        AcquireApp.init(this, “put your account id here”)
    }
}
```

To know more about initialization options [click here](start-using-acquire.md#initialize-acquire-sdk). 

To handle chat events manually [click here](../acquire-apis.md#chat-apis). 

To customize our chat widget [click here](../custom-ui-widget.md#customize-chat-widget).

