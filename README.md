# MyCustomWidgetsLibrary
This is an Android Library for developer to use android customized widgets and change fonts style easily.
<br>
Example is avilable in app module.

<p>
<img src="https://raw.githubusercontent.com/vatsaldesai92/MyCustomWidgetsLibrary/master/app/src/main/assets/images/mycustomwidgets1.png" alt="screenshot" width="270">

<img src="https://raw.githubusercontent.com/vatsaldesai92/MyCustomWidgetsLibrary/master/app/src/main/assets/images/mycustomwidgets2.png" alt="screenshot" width="270">
</p>

##Download

###Gradle dependency:
- Add the following to your project level build.gradle:
~~~
allprojects {
	repositories {
		...
		maven { url "https://jitpack.io" }
	}
}
~~~
- Add this to your app build.gradle:
~~~
dependencies {
	compile 'com.github.vatsaldesai92:MyCustomWidgetsLibrary:1.0.1'
}
~~~

##Usage

- User can can directly change widget fonts by add bellow code in xml.
- Add .ttf file in assets folder.
- app:fontPath contain path of the ttf file that can be from string.xml or direct path of assets.

- if user add .ttf file path in string.xml
~~~
    <string name="font5">verdana.ttf</string>

    <com.desai.vatsal.mycustomwidgets.MyCustomTextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginTop="10dp"
        android:text="my dynamic textview 3"
        app:fontPath="@string/font5" />
~~~
- if user add .ttf file in assets folder
~~~
    <com.desai.vatsal.mycustomwidgets.MyCustomTextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="my dynamic textview 1"
        app:fontPath="verdana.ttf" />
~~~
- if user create folder fonts in assets folder then add .ttf file in it
~~~
    <com.desai.vatsal.mycustomwidgets.MyCustomTextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="my dynamic textview 1"
        app:fontPath="fonts/verdana.ttf" />
~~~

##All Widgets
~~~xml
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:id="@+id/activity_main"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:orientation="vertical">

            <com.desai.vatsal.mycustomwidgets.MyCustomTextView
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:text="my dynamic textview 1"
                app:fontPath="cambriai.ttf" />

            <com.desai.vatsal.mycustomwidgets.MyCustomEditText
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:layout_marginTop="10dp"
                android:hint="my dynamic edittext 1"
                app:fontPath="@string/font4" />

            <com.desai.vatsal.mycustomwidgets.MyCustomRadioButton
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:layout_marginTop="10dp"
                android:text="my dynamic radio button 2"
                app:fontPath="verdana.ttf" />

            <com.desai.vatsal.mycustomwidgets.MyCustomCheckBox
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:layout_marginTop="10dp"
                android:text="my dynamic checkbox 1"
                app:fontPath="@string/font4" />

            <com.desai.vatsal.mycustomwidgets.MyCustomButton
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:layout_marginTop="10dp"
                android:text="my dynamic button 2"
                app:fontPath="verdana.ttf" />

            <com.desai.vatsal.mycustomwidgets.MyCustomAutoCompleteTextView
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:layout_marginTop="10dp"
                android:text="my dynamic auto complete textview 1"
                app:fontPath="@string/font5" />

            <com.desai.vatsal.mycustomwidgets.MyCustomCheckedTextView
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:layout_marginTop="10dp"
                android:text="my dynamic checked textview 1"
                app:fontPath="cambriai.ttf" />

            <com.desai.vatsal.mycustomwidgets.MyCustomMultiAutoCompleteTextView
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:layout_marginTop="10dp"
                android:text="my dynamic multi auto complete textview 1"
                app:fontPath="@string/font3" />

            <com.desai.vatsal.mycustomwidgets.MyCustomSwitch
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:layout_marginTop="10dp"
                android:text="my dynamic switch 1"
                app:fontPath="@string/font3" />

            <com.desai.vatsal.mycustomwidgets.MyCustomToggleButton
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:layout_marginTop="10dp"
                android:text="my dynamic toggle button 1"
                app:fontPath="@string/font3" />

</LinearLayout>
~~~

##License
~~~
    Apache Version 2.0

    Copyright 2016.

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
~~~
