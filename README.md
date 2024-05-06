
# Ex.No:10 To create a option menu to display menu items.


## AIM:

To create a option menu to display menu items using Android Studio.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio

## ALGORITHM:



## PROGRAM:
```
/*
Program to print the text “optionmenu”.
Developed by:VISHVA V
Registeration Number :212222040182
*/
```
In activity_main.xml
```
<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <androidx.appcompat.widget.Toolbar
        android:id="@+id/toolbar"
        android:layout_width="match_parent"
        android:layout_height="?attr/actionBarSize"
        android:background="?attr/colorPrimary"
        app:title="Options Menu Example"
        app:titleTextColor="@android:color/white" />

</RelativeLayout>
```
In MainActivity.java
```
package com.example.menuinandroid;

import androidx.appcompat.app.AppCompatActivity;
import android.os.Bundle;
import android.view.Menu;
import android.view.MenuInflater;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        // Set the toolbar as the action bar
        androidx.appcompat.widget.Toolbar toolbar = findViewById(R.id.toolbar);
        setSupportActionBar(toolbar);
    }

    @Override
    public boolean onCreateOptionsMenu(Menu menu) {
        MenuInflater inflater = getMenuInflater();
        inflater.inflate(R.menu.option, menu);
        return true;
    }
}
```
In menu/option.xml
```
<?xml version="1.0" encoding="utf-8"?>
<menu xmlns:android="http://schemas.android.com/apk/res/android">
    <item
        android:id="@+id/action_item1"
        android:title="Item 1" />
    <item
        android:id="@+id/action_item2"
        android:title="Item 2" />
    <item
        android:id="@+id/action_item3"
        android:title="Item 3" />
</menu>
```

## OUTPUT
![WhatsApp Image 2024-05-06 at 08 28 21_54cecb08](https://github.com/VISHVA12300/menuinandroid/assets/119404426/23c5d8b2-89b0-4825-8347-d8ad8fcb79bc)
![WhatsApp Image 2024-05-06 at 08 28 19_781c2f6c](https://github.com/VISHVA12300/menuinandroid/assets/119404426/5ad43606-0336-4555-997f-65536ece3f99)





## RESULT
Thus a Simple Android Application to create a option menu to display menu items using Android Studio is developed and executed successfully.
