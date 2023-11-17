# Ex.No:10 To create a option menu to display menu items.


## AIM:

To create a option menu to display menu items using Android Studio.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio

## ALGORITHM:
```
Open Android Studio and then click on File -> New -> New project.
Then type the Application name as HelloWorld and click Next.
Then select the Minimum SDK as shown below and click Next.
Then select the Empty Activity and click Next. Finally click Finish.
Design layout in activity_main.xml.
Display message give in MainActivity file.
Save and run the application.
```

## PROGRAM:
```
/*
Program to print the text “optionmenu”.
Developed by:Suryanarayanan.S
Registeration Number :212221220053
*/
```
## activity_main.xml
```
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hello World!"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

</androidx.constraintlayout.widget.ConstraintLayout>
```
## MainActivity.java
```
package com.example.myapplication;

import androidx.appcompat.app.AppCompatActivity;
import android.os.Bundle;
import android.view.Menu;
import android.view.MenuInflater;

public class MainActivity extends AppCompatActivity {
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
    }
    @Override
    public boolean onCreateOptionsMenu(Menu menu) {
        MenuInflater m = getMenuInflater();
        m.inflate(R.menu.option,menu);
        return true;
    }
}
```
## option.xml
```
<?xml version="1.0" encoding="utf-8"?>
<menu xmlns:android="http://schemas.android.com/apk/res/android">
    <item android:title="Item 1" />
    <item android:title="Item 2" />
    <item android:title="Item 3" />
</menu>
```

## OUTPUT
![image](https://github.com/Naveen-154/Mobile-Application-Development/assets/114643271/eb63157d-bb26-49c6-a99f-0dfc3416ceba)
![image](https://github.com/Naveen-154/Mobile-Application-Development/assets/114643271/3a5a7ca3-ceb8-4591-9b11-addc01257f41)




## RESULT
Thus a Simple Android Application to create a option menu to display menu items using Android Studio is developed and executed successfully.
