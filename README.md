# Ex.No:1 To create a HelloWorld Activity using all lifecycles methods to display messages.

## DATE : 26.10.26

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


Program to print the text “Hello World”.
```
Developed by: GURUPARAN G
Registeration Number : 212224220030
```

## MAINACTIVITY.JAVA:

```
package com.example.myapplication ;

import android.os.Bundle;
import android.widget.Toast;

import androidx.activity.EdgeToEdge;
import androidx.appcompat.app.AppCompatActivity;
import androidx.core.graphics.Insets;
import androidx.core.view.ViewCompat;
import androidx.core.view.WindowInsetsCompat;

import com.example.myapplication.R;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Toast t = Toast.makeText(getApplicationContext(),"onCreate Called", Toast.LENGTH_LONG);
        t.show();

    }
    protected void onStart(){
        super.onStart();
        Toast t = Toast.makeText(getApplicationContext(),"onStart Called", Toast.LENGTH_LONG);
        t.show();
    }
    protected void onRestart(){
        super.onRestart();
        Toast t = Toast.makeText(getApplicationContext(), "onRestart Called", Toast.LENGTH_LONG);
        t.show();
    }
    protected void onPause(){
        super.onPause();
        Toast t = Toast.makeText(getApplicationContext(), "onPause Called", Toast.LENGTH_LONG);
        t.show();
    }
    protected void onResume(){
        super.onResume();
        Toast t = Toast.makeText(getApplicationContext(), "onResume Called", Toast.LENGTH_LONG);
        t.show();
    }
    protected void onStop(){
        super.onStop();
        Toast t = Toast.makeText(getApplicationContext(), "onStop Called", Toast.LENGTH_LONG);
        t.show();
    }
    protected void onDestroy(){
        super.onDestroy();
        Toast t = Toast.makeText(getApplicationContext(), "onDestroy Called", Toast.LENGTH_LONG);
        t.show();
    }


}
```


## ACTIVITY_MAIN.XML:

```
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:id="@+id/main"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="#65F43688"
    tools:context=".MainActivity">

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:fontFamily="sans-serif-black"
        android:text="Welcome to Guru's Android"
        android:textSize="16sp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

</androidx.constraintlayout.widget.ConstraintLayout>

```



## OUTPUT


## FIRST MAIN SCREEN
<img width="1917" height="1198" alt="Screenshot 2026-10-26 233131" src="https://github.com/user-attachments/assets/e5d004d9-a24c-4e9c-8dde-67f38e906cce" />


## onCreate()
<img width="1917" height="1198" alt="Screenshot 2026-10-26 233332" src="https://github.com/user-attachments/assets/4c844ef8-7e2a-4087-a833-cdb8cdba302c" />


## onResume()
<img width="1917" height="1198" alt="Screenshot 2026-10-26 233344" src="https://github.com/user-attachments/assets/112cbb2a-aae2-4979-80b0-e4334ce185cc" />



## onStart()
<img width="1917" height="1198" alt="Screenshot 2026-10-26 233429" src="https://github.com/user-attachments/assets/f2051599-5ec6-4e9f-9b36-d1366285505a" />


## onPause() 
<img width="1917" height="1198" alt="Screenshot 2026-10-26 233634" src="https://github.com/user-attachments/assets/84c2ed63-f03e-4e10-81c1-fb4b9af21252" />



## onRestart()
<img width="1917" height="1197" alt="Screenshot 2026-10-26 233700" src="https://github.com/user-attachments/assets/7d94ba11-5c51-446c-8cf5-6668fb47a79d" />


## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
