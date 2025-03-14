- 👋 Hi, I’m @Yg46eagle
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
Yg46eagle/Yg46eagle is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
Overview
Bundled GIFLib via JNI is used to render frames. This way should be more efficient than WebView or Movie classes.

Javadoc
Setup
Gradle (Android Studio)
Insert the following dependency to build.gradle file of your project.

dependencies {
    implementation 'pl.droidsonroids.gif:android-gif-drawable:1.2.29'
}
Note that Maven central repository should be defined eg. in top-level build.gradle like this:

buildscript {
    repositories {
        mavenCentral()
    }
}
allprojects {
    repositories {
        mavenCentral()
    }
}
Gradle, snapshot repository
Current development builds (build from dev branch) are published to OSS snapshot repository. To use them, specify repository URL in repositories block:

repositories {
    mavenCentral()
    maven { url "https://oss.sonatype.org/content/repositories/snapshots" }
}
dependencies {
    implementation 'pl.droidsonroids.gif:android-gif-drawable:1.2.+'
}
Maven dependency
<dependency>
    <groupId>pl.droidsonroids.gif</groupId>
    <artifactId>android-gif-drawable</artifactId>
    <version>insert latest version here</version>
    <type>aar</type>
</dependency>