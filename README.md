<img src="images/Calc_Vid.gif" width="300"  />  <br><br>
# Calculator App
Here we are going to see how to make a simple calculator app in kotlin using android studio <br><br>
 ## Creating project
 * Launch android studio<br><br>
 ![](/images/cal1.png) <br><br>
 * Click on `Create New Project`<br><br>
 ![](/images/cal2.png) <br><br>
 * Select `Empty Activity`
 * Click on `Next`<br><br>
 ![](/images/cal3.png) <br><br>
 * Give a Name , Package name 
 * Select Language as `Kotlin`
 * Change Save location if required
 * Select Minimum SDK as required or Select API21(I need  to run app in Android 5.0(lollipop) and above so i choose API21)
 * Click `Finish`<br><br>
 ![](/images/cal4.png) <br><br>
 You can see screen as shown above after build <br><br> 
  ![](/images/cal10.png) <br><br>
 * Open colors.xml by `Android` >> `values` >> `colors.xml` , Double click on colors.xml
 * Make it blank . Copy the code below <br><br>
 ```xml
<?xml version="1.0" encoding="utf-8"?>
<resources>
    <color name="purple_200">#FFBB86FC</color>
    <color name="purple_500">#FF6200EE</color>
    <color name="purple_700">#FF3700B3</color>
    <color name="teal_200">#FF03DAC5</color>
    <color name="teal_700">#FF018786</color>
    <color name="black">#FF000000</color>
    <color name="white">#FFFFFFFF</color>
    <color name="red">#FF3131</color>
    <color name="pink">#FFC0CB</color>
    <color name="orange">#FFA500</color>
    <color name="neon_green">#39FF14</color>
</resources>
```
<br><br>
* Paste it in colors.xml file
* Click on Sync Project with Gradle Files  ![](/images/cal12.png)<br><br>
![](/images/cal7.png) <br><br>
* Open themes.xml by `Android` >> `themes` >> `themes.xml` , Double click on themes.xml
* Make it blank . Copy the code below <br><br>
 ```xml
<resources xmlns:tools="http://schemas.android.com/tools">
    <!-- Base application theme. -->
    <style name="Theme.Calc" parent="Theme.MaterialComponents.DayNight.DarkActionBar">
        <!-- Primary brand color. -->
        <item name="colorPrimary">@color/purple_500</item>
        <item name="colorPrimaryVariant">@color/purple_700</item>
        <item name="colorOnPrimary">@color/white</item>
        <!-- Secondary brand color. -->
        <item name="colorSecondary">@color/neon_green</item>
        <item name="colorSecondaryVariant">@color/neon_green</item>
        <item name="colorOnSecondary">@color/black</item>
        <!-- Status bar color. -->
        <item name="android:statusBarColor" tools:targetApi="l">?attr/colorPrimaryVariant</item>
        <!-- Customize your theme here. -->
    </style>
    <style name="splash_screen_theme" parent="Theme.MaterialComponents.Light.NoActionBar">
        <item name="android:windowBackground">@drawable/splash_screen</item>
        <item name="android:statusBarColor">@color/white</item>
    </style>
</resources>
```
<br><br>
* Paste it in themes.xml file
* Click on Sync Project with Gradle Files  ![](/images/cal12.png)<br><br>
![](/images/cal8.png)<br><br>
* Open splash_screen.xml by `Android` >> `drawable` >> `splash_screen.xml` , Double click on splash_screen.xml
* Make it blank . Copy the code below <br><br>
```xml
<?xml version="1.0" encoding="utf-8"?>
<layer-list xmlns:android="http://schemas.android.com/apk/res/android">
<item android:drawable="@color/white"/>
    <item android:drawable="@drawable/ic_logo" android:gravity="center"/>
</layer-list>
```
<br><br>
* Paste it in themes.xml file
* Click on Sync Project with Gradle Files  ![](/images/cal12.png)<br><br>
![](/images/cal11.png)<br><br>
* Open styles.xml by `Android` >> `values` >> `styles.xml` , Double click on style.xml
* Make it blank . Copy the code below <br><br>
```xml
<?xml version="1.0" encoding="utf-8"?>
<resources>
    <style name="Button_Style" parent="Widget.AppCompat.Button.Colored">
        <item name="android:background">@color/white</item>
        <item name="android:textSize">24sp</item>
        <item name="android:textColor">@color/black</item>
        <item name="android:gravity">center</item>
    </style>
</resources>
```
