# Map Item Navigation
Recently in one of the projects needed to create a dynamic map where a list of stores that were to user location 1Km should be displayed. I took the day today to move all the code developed for a separate project, I will share it with you in this article.

| Gif | Video |
| --- | --- |
| ![ContactPikerAnimated](https://meucomercioeletronico.com/tutorial/MapItemNavigationEn.gif)  | [![VIDEO](https://img.youtube.com/vi/rq8Rd_VVBAg/0.jpg)](https://www.youtube.com/watch?v=rq8Rd_VVBAg) |


## Instalação e uso
Just import the Git project for your favorite editor and make the exchange of API_KEY.

To do this edit the file AndroidManifest.xml line 25.
```
<?xml version="1.0" encoding="utf-8"?>
<manifest xmlns:android="http://schemas.android.com/apk/res/android"
    package="guilherme.com.br.mapitemnavigation">


    <!-- ========================= Global Permissions ====================================== -->
    <uses-permission android:name="android.permission.ACCESS_COARSE_LOCATION" />
    <uses-permission android:name="android.permission.ACCESS_FINE_LOCATION" />
    <uses-permission android:name="android.permission.INTERNET" />


    <application
        android:name=".Application"
        android:allowBackup="true"
        android:icon="@mipmap/ic_launcher"
        android:label="@string/app_name"
        android:supportsRtl="true"
        android:theme="@style/AppTheme">

        <!-- ========================= Google Maps Specific ===================================== -->
        <!--Change Here Your APi Key em: -->
        <!-- https://developers.google.com/maps/documentation/android-api/signup -->
        <meta-data
            android:name="com.google.android.maps.v2.API_KEY"
            android:value="YOUR_API_KEY_HERE" />

        <activity
            android:name=".MainActivity"
            android:label="@string/app_name"
            android:theme="@style/AppTheme.NoActionBar">
            <intent-filter>
                <action android:name="android.intent.action.MAIN" />
                <category android:name="android.intent.category.LAUNCHER" />
            </intent-filter>
        </activity>

        <!-- ========================= ExpandedMapActivity Activities ===================================== -->

        <activity
            android:name=".ExpandedMapActivity"
            android:label="ExpandedMapActivity"
            android:screenOrientation="portrait">
        </activity>


    </application>

</manifest>
```

If you don't have the API KEY, this link will help you:
https://developers.google.com/maps/documentation/android-api/signup

## Thanks
I hope it helped you!

I am a willingness to ask questions:
guilhermeborgesbastos@gmail.com

## Contact
[![VIDEO](https://media.licdn.com/mpr/mpr/shrinknp_100_100/AAEAAQAAAAAAAAgiAAAAJGMwMTQwNTMyLTU2N2EtNDM1NS1iZDMxLTI2ZjVhZDRlNjM2Mw.jpg)](https://www.facebook.com/AndroidNaPratica)
