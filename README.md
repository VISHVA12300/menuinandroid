
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

![Screenshot 2024-05-08 103616](https://github.com/VISHVA12300/menuinandroid/assets/119404426/a5f2098b-ab34-40d5-ae64-27263e205968)

![Screenshot 2024-05-08 103624](https://github.com/VISHVA12300/menuinandroid/assets/119404426/bbf62c5a-3f63-417a-9ac1-118a7666e010)




## RESULT
Thus a Simple Android Application to create a option menu to display menu items using Android Studio is developed and executed successfully.
