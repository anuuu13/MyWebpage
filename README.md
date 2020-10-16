<?xml version="1.0" encoding="utf-8"?> 
<androidx.constraintlayout.widget.ConstraintLayout
	xmlns:android="http://schemas.android.com/apk/res/android"
	xmlns:app="http://schemas.android.com/apk/res-auto"
	xmlns:tools="http://schemas.android.com/tools"
	android:layout_width="match_parent"
	android:layout_height="match_parent"
	android:background="#8BC34A"
	android:backgroundTint="@android:color/darker_gray"
	tools:context=".MainActivity"> 

	<!-- Text View to display "myFirstApp "-->
	<TextView
		android:id="@+id/textView"
		android:layout_width="133dp"
		android:layout_height="28dp"
		android:layout_marginStart="139dp"
		android:layout_marginLeft="139dp"
		android:layout_marginTop="16dp"
		android:layout_marginEnd="139dp"
		android:layout_marginRight="139dp"
		android:layout_marginBottom="559dp"

		<!-- providing the green colour to the background -->
		android:background="#0F9D58" 

		android:text="myFirstApp" 
		android:textAppearance="@style/TextAppearance.AppCompat.Medium" 
		app:layout_constraintBottom_toBottomOf="parent" 
		app:layout_constraintEnd_toEndOf="parent" 
		app:layout_constraintStart_toStartOf="parent" 
		app:layout_constraintTop_toTopOf="parent" /> 

	<!-- Text View to display our basic heading of "calculator"-->
	<TextView
		android:layout_width="194dp"
		android:layout_height="43dp"
		android:layout_marginStart="114dp"
		android:layout_marginLeft="114dp"
		android:layout_marginTop="58dp"
		android:layout_marginEnd="103dp"
		android:layout_marginRight="103dp"
		android:layout_marginBottom="502dp"
		android:scrollbarSize="30dp"
		android:text=" Calculator"
		android:textAppearance="@style/TextAppearance.AppCompat.Body1"
		android:textSize="30dp"
		app:layout_constraintBottom_toBottomOf="parent"
		app:layout_constraintEnd_toEndOf="parent"
		app:layout_constraintStart_toStartOf="parent"
		app:layout_constraintTop_toTopOf="parent" /> 

	<!-- Edit Text View to input the values -->
	<EditText
		android:id="@+id/num1"
		android:layout_width="364dp"
		android:layout_height="28dp"
		android:layout_marginStart="72dp"
		android:layout_marginTop="70dp"
		android:layout_marginEnd="71dp"
		android:layout_marginBottom="416dp"
		android:background="@android:color/white"
		android:ems="10"
		android:hint="Number1(0)"
		android:inputType="number"
		app:layout_constraintBottom_toBottomOf="parent"
		app:layout_constraintEnd_toEndOf="parent"
		app:layout_constraintStart_toStartOf="parent"
		app:layout_constraintTop_toTopOf="parent" /> 

	<!-- Edit Text View to input 2nd value-->
	<EditText
		android:id="@+id/num2"
		android:layout_width="363dp"
		android:layout_height="30dp"
		android:layout_marginStart="72dp"
		android:layout_marginTop="112dp"
		android:layout_marginEnd="71dp"
		android:layout_marginBottom="374dp"
		android:background="@android:color/white"
		android:ems="10"
		android:hint="number2(0)"
		android:inputType="number"
		app:layout_constraintBottom_toBottomOf="parent"
		app:layout_constraintEnd_toEndOf="parent"
		app:layout_constraintStart_toStartOf="parent"
		app:layout_constraintTop_toTopOf="parent" /> 

	<!-- Text View to display result -->
	<TextView
		android:id="@+id/result"
		android:layout_width="356dp"
		android:layout_height="71dp"
		android:layout_marginStart="41dp"
		android:layout_marginTop="151dp"
		android:layout_marginEnd="48dp"
		android:layout_marginBottom="287dp"
		android:background="@android:color/white"
		android:text="result"
		android:textColorLink="#673AB7"
		android:textSize="25sp"
		app:layout_constraintBottom_toBottomOf="parent"
		app:layout_constraintEnd_toEndOf="parent"
		app:layout_constraintStart_toStartOf="parent"
		app:layout_constraintTop_toTopOf="parent" /> 

	<!-- A button to perform 'sum' operation -->
	<Button
		android:id="@+id/sum"
		android:layout_width="wrap_content"
		android:layout_height="wrap_content"
		android:layout_marginStart="16dp"
		android:layout_marginTop="292dp"
		android:layout_marginEnd="307dp"
		android:layout_marginBottom="263dp"
		android:backgroundTint="@android:color/holo_red_light"
		android:onClick="doSum"
		android:text="+"
		app:layout_constraintBottom_toBottomOf="parent"
		app:layout_constraintEnd_toEndOf="parent"
		app:layout_constraintStart_toStartOf="parent"
		app:layout_constraintTop_toTopOf="parent" /> 

	<!-- A button to perform subtraction operation. -->
	<Button
		android:id="@+id/sub"
		android:layout_width="wrap_content"
		android:layout_height="wrap_content"
		android:layout_marginStart="210dp"
		android:layout_marginTop="292dp"
		android:layout_marginEnd="113dp"
		android:layout_marginBottom="263dp"
		android:backgroundTint="@android:color/holo_red_light"
		android:onClick="doSub"
		android:text="-"
		app:layout_constraintBottom_toBottomOf="parent"
		app:layout_constraintEnd_toEndOf="parent"
		app:layout_constraintStart_toStartOf="parent"
		app:layout_constraintTop_toTopOf="parent" /> 
	
	<!-- A button to perform division. -->
	<Button
		android:id="@+id/div"
		android:layout_width="wrap_content"
		android:layout_height="wrap_content"
		android:layout_marginStart="307dp"
		android:layout_marginTop="292dp"
		android:layout_marginEnd="16dp"
		android:layout_marginBottom="263dp"
		android:backgroundTint="@android:color/holo_red_light"
		android:onClick="doDiv"
		android:text="/"
		app:layout_constraintBottom_toBottomOf="parent"
		app:layout_constraintEnd_toEndOf="parent"
		app:layout_constraintHorizontal_bias="0.0"
		app:layout_constraintStart_toStartOf="parent"
		app:layout_constraintTop_toTopOf="parent" /> 
	
	<!-- A button to perform multiplication. -->
	<Button
		android:id="@+id/mul"
		android:layout_width="wrap_content"
		android:layout_height="wrap_content"
		android:layout_marginStart="16dp"
		android:layout_marginTop="356dp"
		android:layout_marginEnd="307dp"
		android:layout_marginBottom="199dp"
		android:backgroundTint="@android:color/holo_red_light"
		android:onClick="doMul"
		android:text="x"
		app:layout_constraintBottom_toBottomOf="parent"
		app:layout_constraintEnd_toEndOf="parent"
		app:layout_constraintStart_toStartOf="parent"
		app:layout_constraintTop_toTopOf="parent" /> 
	
	<!-- A button to perform a modulus function. -->
	<Button
		android:id="@+id/button"
		android:layout_width="92dp"
		android:layout_height="48dp"
		android:layout_marginStart="113dp"
		android:layout_marginTop="356dp"
		android:layout_marginEnd="206dp"
		android:layout_marginBottom="199dp"
		android:backgroundTint="@android:color/holo_red_light"
		android:onClick="doMod"
		android:text="%(mod)"
		app:layout_constraintBottom_toBottomOf="parent"
		app:layout_constraintEnd_toEndOf="parent"
		app:layout_constraintStart_toStartOf="parent"
		app:layout_constraintTop_toTopOf="parent" /> 
	
	<!-- A button to perform a power function. -->
	<Button
		android:id="@+id/pow"
		android:layout_width="wrap_content"
		android:layout_height="wrap_content"
		android:layout_marginStart="113dp"
		android:layout_marginTop="292dp"
		android:layout_marginEnd="210dp"
		android:layout_marginBottom="263dp"
		android:backgroundTint="@android:color/holo_red_light"
		android:onClick="doPow"
		android:text="n1^n2"
		app:layout_constraintBottom_toBottomOf="parent"
		app:layout_constraintEnd_toEndOf="parent"
		app:layout_constraintStart_toStartOf="parent"
		app:layout_constraintTop_toTopOf="parent" /> 

</androidx.constraintlayout.widget.ConstraintLayout> 


package com.example.gfg_my_first_app; 

import androidx.appcompat.app.AppCompatActivity; 

import android.os.Bundle; 
import android.view.View; 
import android.widget.Button; 
import android.widget.EditText; 
import android.widget.TextView; 

public class MainActivity extends AppCompatActivity { 

	EditText e1, e2; 
	TextView t1; 
	int num1, num2; 

	@Override
	protected void onCreate(Bundle savedInstanceState) 
	{ 
		super.onCreate(savedInstanceState); 

		setContentView(R.layout.activity_main); 
	} 

	// a public method to get the input numbers 
	public boolean getNumbers() 
	{ 

		// defining the edit text 1 to e1 
		e1 = (EditText)findViewById(R.id.num1); 

		// defining the edit text 2 to e2 
		e2 = (EditText)findViewById(R.id.num2); 

		// defining the text view to t1 
		t1 = (TextView)findViewById(R.id.result); 

		// taking input from text box 1 
		s1 = e1.getText().toString(); 

		// taking input from text box 2 
		s2 = e2.getText().toString(); 

		// condition to check if box is not empty 
		if ((s1.equals(null) && s2.equals(null)) 
			|| (s1.equals("") && s2.equals(""))) { 

			String result = "Please enter a value"; 
			t1.setText(result); 

			return false; 
		} 
		else { 
			// converting string to int. 
			num1 = Integer.parseInt(e1.getText().toString()); 

			// converting string to int. 
			num2 = Integer.parseInt(e2.getText().toString()); 
		} 

		return true; 
	} 

	// a public method to perform addition 
	public void doSum(View v) 
	{ 

		// get the input numbers 
		if (getNumbers()) { 
			int sum = num1 + num2; 
			t1.setText(Integer.toString(sum)); 
		} 
	} 

	// a public method to perform power function 
	public void doPow(View v) 
	{ 

		// get the input numbers 
		if (getNumbers()) { 
			double sum = Math.pow(num1, num2); 
			t1.setText(Double.toString(sum)); 
		} 
	} 

	// a public method to perform subtraction 
	public void doSub(View v) 
	{ 

		// get the input numbers 
		if (getNumbers()) { 
			int sum = num1 - num2; 
			t1.setText(Integer.toString(sum)); 
		} 
	} 

	// a public method to perform multiplication 
	public void doMul(View v) 
	{ 

		// get the input numbers 
		if (getNumbers()) { 
			int sum = num1 * num2; 
			t1.setText(Integer.toString(sum)); 
		} 
	} 
	// a public method to perform Division 
	public void doDiv(View v) 
	{ 

		// get the input numbers 
		if (getNumbers()) { 

			// displaying the text in text view assigned as t1 
			double sum = num1 / (num2 * 1.0); 
			t1.setText(Double.toString(sum)); 
		} 
	} 
	// a public method to perform modulus function 
	public void doMod(View v) 
	{ 

		// get the input numbers 
		if (getNumbers()) { 
			double sum = num1 % num2; 
			t1.setText(Double.toString(sum)); 
		} 
	} 
} 

