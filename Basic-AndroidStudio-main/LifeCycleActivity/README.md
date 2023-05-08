# Ex.No:1 To create a HelloWorld Activity using all lifecycles methods to display messages.

## AIM:

To create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio.

## EQUIPMENTS REQUIRED:

Android Studio(Min.required Artic Fox)

## ALGORITHM:

Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as HelloWorld and click Next.

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Display message give in MainActivity file.

Step 7: Save and run the application.

## PROGRAM:

```
/*
Program to print the text “Hello World”.
Developed by:S.Jeswanth
Registeration Number :212221240042
*/
```

## MainActivity.java:

```
package com.example.helloworld;

import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;
import android.widget.Toast;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);


        Toast toast=Toast.makeText(getApplicationContext(),"Hello world-create",Toast.LENGTH_SHORT);
        toast.show();
    }
    @Override
    protected void onStart() {
        super.onStart();
        Toast toast=Toast.makeText(getApplicationContext(),"Hello world-start",Toast.LENGTH_SHORT);
        toast.show();
    }
    @Override
    protected void onResume() {
        super.onResume();
        Toast toast=Toast.makeText(getApplicationContext(),"Hello world-resume",Toast.LENGTH_SHORT);
        toast.show();
    }
    @Override
    protected void onPause() {
        super.onPause();
        Toast toast=Toast.makeText(getApplicationContext(),"Hello world-pause",Toast.LENGTH_SHORT);
        toast.show();

    }
    @Override
    protected void onStop() {
        super.onStop();
        Toast toast=Toast.makeText(getApplicationContext(),"Hello world-stop",Toast.LENGTH_SHORT);
        toast.show();
    }
    @Override
    protected void onRestart() {
        super.onRestart();
        Toast toast=Toast.makeText(getApplicationContext(),"Hello world-restart",Toast.LENGTH_SHORT);
        toast.show();
    }
    @Override
    protected void onDestroy() {
        super.onDestroy();
        Toast toast=Toast.makeText(getApplicationContext(),"Hello world-destroy",Toast.LENGTH_SHORT);
        toast.show();
    }
}
```

## MainActivity.xml:

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

## OUTPUT

![image](https://user-images.githubusercontent.com/94155480/233846510-01583f4b-e66b-4f3c-9c05-409db6929696.png)
![image](https://user-images.githubusercontent.com/94155480/233846530-a12c0bba-5a23-4729-9c13-a53c61473366.png)
![image](https://user-images.githubusercontent.com/94155480/233846553-2b524ba4-3f06-4d94-8c7f-bea57a8d6f25.png)

## RESULT

Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
