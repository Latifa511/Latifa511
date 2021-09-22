package com.example.helloworldapp

import androidx.appcompat.app.AppCompatActivity
import android.os.Bundle
import android.util.Log

class MainActivity : AppCompatActivity() {
    fun sum (num1 : Int , num2 : Int) : Int {
        return num1+num2
    }

    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        setContentView(R.layout.activity_main)

        var x = 100
        var y = 1000
        var add = sum(x,y)

        if (x<y){
            var massg = "Hello World!"
            Log.d("MainActivity", massg)
            Log.d("MainActivity", "$add")
        }
        else{
            Log.d("MainActivity", "Hello world!")
        }


    }

}
