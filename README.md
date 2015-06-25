# Loyal Native Slider 
[![Android Arsenal](https://img.shields.io/badge/Android%20Arsenal-Loyal%20Native%20Slider-brightgreen.svg?style=flat)](http://android-arsenal.com/details/1/1998)[ ![Download](https://api.bintray.com/packages/jjhesk/maven/library/images/download.svg) ](https://bintray.com/jjhesk/maven/library/_latestVersion)[![Gitter](https://badges.gitter.im/Join Chat.svg)](https://gitter.im/daimajia/AndroidImageSlider?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
 
Master: [![Build Status](https://travis-ci.org/jjhesk/LoyalNativeSlider.svg)](https://travis-ci.org/jjhesk/LoyalNativeSlider)

Dev: [![Build Status](https://travis-ci.org/jjhesk/LoyalNativeSlider.svg?branch=dev)](https://travis-ci.org/jjhesk/LoyalNativeSlider)

This is an amazing image slider for the Android platform. I decided to open source this because there is really not an attractive, convenient slider widget in Android.
 
You can easily load images from an internet URL, drawable, or file. And there are many kinds of amazing animations you can choose. :-D
 
## Demo
 
![](scn/device-2015-06-17-142823.png)
![](scn/device-2015-06-17-150718.png)
![](scn/device-2015-06-17-150829.png)

from daimajia [Download Apk](https://github.com/daimajia/AndroidImageSlider/releases/download/v1.0.8/demo-1.0.8.apk)
 
## Usage

### Step 1

#### Gradle
[ ![Download](https://api.bintray.com/packages/jjhesk/maven/library/images/download.svg) ](https://bintray.com/jjhesk/maven/library/_latestVersion)
```groovy

dependencies {
    compile 'com.android.support:appcompat-v7:22.1.1'
    compile 'com.android.support:support-v4:22.1.1'
    compile 'com.squareup.picasso:picasso:2.5.2'
    compile 'com.nineoldandroids:library:2.4.0'

    compile 'com.hkm.loyalslider:library:1.2.1@aar'
}

```


#### Maven

```xml
<dependency>
    <groupId>com.squareup.picasso</groupId>
    <artifactId>picasso</artifactId>
    <version>2.5.2</version>
</dependency>
<dependency>
    <groupId>com.nineoldandroids</groupId>
    <artifactId>library</artifactId>
    <version>2.4.0</version>
</dependency>
<dependency>
    <groupId>com.hkm.loyalslider</groupId>
    <artifactId>library</artifactId>
    <version>1.2.1</version>
    <type>apklib</type>
</dependency>
```

#### Eclipse

For Eclipse users, I provided a sample project which orgnized as Eclipse way. You can download it from [here](https://github.com/daimajia/AndroidImageSlider/releases/download/v1.0.9/AndroidImageSlider-Eclipse.zip), and make some changes to fit your project.

Notice: It's the version of 1.0.9, it may not update any more. You can update manually by yourself.

For Eclipse project, you might need to with the parent project from daimajia.

### Step 2

Add permissions (if necessary) to your `AndroidManifest.xml`

```xml
<!-- if you want to load images from the internet -->
<uses-permission android:name="android.permission.INTERNET" /> 

<!-- if you want to load images from a file OR from the internet -->
<uses-permission android:name="android.permission.READ_EXTERNAL_STORAGE" />
```

**Note:** If you want to load images from the internet, you need both the `INTERNET` and `READ_EXTERNAL_STORAGE` permissions to allow files from the internet to be cached into local storage.

If you want to load images from drawable, then no additional permissions are necessary.

### Step 3

Add the Slider to your layout:
 
```java
<com.hkm.slider.SliderLayout
        android:id="@+id/slider"
        android:layout_width="match_parent"
        android:layout_height="200dp"
/>
```        
 
There are some default indicators. If you want to use a provided indicator:
 
```java
<com.hkm.slider.Indicators.PagerIndicator
        android:id="@+id/custom_indicator"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:gravity="center"
        />
```

[Code example](https://github.com/jjhesk/LoyalNativeSlider/blob/master/demo/src/main/java/com/daimajia/slider/demo/MainActivity.java)
 
====

## Advanced usage
Visit the Transform [Wiki](https://github.com/jjhesk/LoyalNativeSlider/wiki)
Please visit [Wiki](https://github.com/daimajia/AndroidImageSlider/wiki) for the mother library
 
## Thanks for the Reference

- [Picasso](https://github.com/square/picasso)
- [NineOldAndroids](https://github.com/JakeWharton/NineOldAndroids)
- [ViewPagerTransforms](https://github.com/ToxicBakery/ViewPagerTransforms)
- [Android Image Slider](https://github.com/daimajia/AndroidImageSlider)

If there are someone who I do not mention here, please accept my sincere appologies and tell me.

###Donation:
Donate $9.99: [![$9.99](http://i.imgur.com/wUWK6e1.jpg)](https://www.paypal.com/cgi-bin/webscr?cmd=_xclick&business=ooxfordck@gmail.com&currency_code=USD&amount=9.99&return=&item_name=LoyalSliderDonation)

Donate $19.99: [![$19.99](http://i.imgur.com/wUWK6e1.jpg)](https://www.paypal.com/cgi-bin/webscr?cmd=_xclick&business=ooxfordck@gmail.com&currency_code=USD&amount=19.99&return=&item_name=LoyalSliderDonation)

Donate $39.99: [![$39.99](http://i.imgur.com/wUWK6e1.jpg)](https://www.paypal.com/cgi-bin/webscr?cmd=_xclick&business=ooxfordck@gmail.com&currency_code=USD&amount=39.99&return=&item_name=LoyalSliderDonation)

Donate $59.99: [![$59.99](http://i.imgur.com/wUWK6e1.jpg)](https://www.paypal.com/cgi-bin/webscr?cmd=_xclick&business=ooxfordck@gmail.com&currency_code=USD&amount=59.99&return=&item_name=LoyalSliderDonation)


Open Donation - USD: [![OPEN](http://i.imgur.com/wUWK6e1.jpg)](https://www.paypal.com/cgi-bin/webscr?cmd=_xclick&business=ooxfordck@gmail.com&currency_code=USD&amount=&return=&item_name=LoyalSliderDonation)

Open Donation - HKD: [![OPEN](http://i.imgur.com/wUWK6e1.jpg)](https://www.paypal.com/cgi-bin/webscr?cmd=_xclick&business=ooxfordck@gmail.com&currency_code=HKD&amount=&return=&item_name=LoyalSliderDonation)

License
--------

    Copyright 2015 JJHesk

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.


##About me
