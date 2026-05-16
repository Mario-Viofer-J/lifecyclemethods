# Ex.No:1 To create a HelloWorld Activity using all lifecycles methods to display messages.

## AIM:
To create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio

## ALGORITHM:

Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as HelloWorld and click Next. 

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Display message give in MainActivity file.

Step 7: Save and run the application.

## PROGRAM:

## Program to print the text “Hello World”.
### Developed by: Mario Viofer J
### Registeration Number : 212223100032

### activity_main.xml
```
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:id="@+id/main"
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
### MainActivity.Java
```
package com.example.activitylifecyclemethods;

import android.os.Bundle;
import android.widget.Toast;
import androidx.appcompat.app.AppCompatActivity;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Toast.makeText(this, "onCreate Called", Toast.LENGTH_LONG).show();
    }

    @Override
    protected void onStart() {
        super.onStart();
        Toast.makeText(this, "onStart Called", Toast.LENGTH_LONG).show();
    }

    @Override
    protected void onRestart() {
        super.onRestart();
        Toast.makeText(this, "onRestart Called", Toast.LENGTH_LONG).show();
    }

    @Override
    protected void onResume() {
        super.onResume();
        Toast.makeText(this, "onResume Called", Toast.LENGTH_LONG).show();
    }

    @Override
    protected void onPause() {
        super.onPause();
        Toast.makeText(this, "onPause Called", Toast.LENGTH_LONG).show();
    }

    @Override
    protected void onStop() {
        super.onStop();
        Toast.makeText(this, "onStop Called", Toast.LENGTH_LONG).show();
    }

    @Override
    protected void onDestroy() {
        super.onDestroy();
        Toast.makeText(this, "onDestroy Called", Toast.LENGTH_LONG).show();
    }
}

```

## OUTPUT
### MainActivity.java
<img width="1012" height="963" alt="image" src="https://github.com/user-attachments/assets/203e26e2-2e02-4c7a-82a1-a603f0d8cd26" />


### activity_main.xml
<img width="1048" height="567" alt="image" src="https://github.com/user-attachments/assets/35f7425b-5caa-40a0-9b8f-d124b6f42c06" />


### onCreate()
<img width="1503" height="956" alt="image" src="https://github.com/user-attachments/assets/6542f8fc-91c3-47df-9bdd-88d4b26bf3c8" />


### onStart()
<img width="1505" height="949" alt="image" src="https://github.com/user-attachments/assets/b00faa81-490e-46e1-a0d0-3cb446a96e25" />


### onResume()
<img width="1505" height="951" alt="image" src="https://github.com/user-attachments/assets/1abc9294-475b-4040-895b-ee61f502d102" />


### onRestart()
<img width="1512" height="955" alt="image" src="https://github.com/user-attachments/assets/fedb46fa-d228-4821-8925-9012dcf5d98c" />


### onPause()
<img width="1508" height="952" alt="image" src="https://github.com/user-attachments/assets/0fc8ce49-0896-499d-a125-c8446cdf2c3a" />


## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
