package com.example.rukmi.refreshdemo;

import android.os.Handler;
import android.support.v7.app.AppCompatActivity;
import android.os.Bundle;
import android.view.View;
import android.widget.Button;
import android.widget.TextView;
import android.widget.Toast;

public class MainActivity extends AppCompatActivity {
    private Handler handler;

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        handler = new Handler();
        Runnable r = new Runnable() {
            public void run() {
                Toast.makeText(MainActivity.this, "Refresh", Toast.LENGTH_SHORT).show();
                handler.postDelayed(this, 5000); //  delay one second before updating the number
            }
        };
        handler.postDelayed(r, 5000); // delay one second before updating the number
    }
}

