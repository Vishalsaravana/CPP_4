# C++ CLASS OBJECT CONVERSION

## PROGRAM STATEMENT :

To write a CPP Program for Class conversion that can be achieved by conversion function which is done by the use of operator overloading

## ALGORITHM:  

1.	Start the program.
2.	Define a class Class_type_one with a private float variable a to store a float value. Provide a default constructor to initialize a to 0.0, a parameterized constructor to initialize a with a specific float value, a get method to return a, and a display method to print a.
3.	Define another class Class_type_two with a private float variable b to store the converted value. Overload the assignment operator (=) to convert an object of Class_type_one to Class_type_two by assigning a's value to b. Include a display method to print b.
4.	In the main function, read a float input from the user and create an object obj1 of Class_type_one initialized with this input.
5.	Create an object obj2 of Class_type_two, and use the overloaded assignment operator to assign obj1 to obj2.
6.	Call the display method for both obj1 and obj2 to display the values stored in Class_type_one and Class_type_two, respectively.
7.	End the program.

## PROGRAM:
```
#include <bits/stdc++.h> #include <string.h> using namespace std;
//type to which it will be converted
// Class to storetheoriginalfloat value class Class_type_one
{
float a; // Private membervariable to storethe float value

public:
// Constructorto initialize thevalue of'a' Class_type_one()
{
a= 0.0; // Initialize withdefault value 0.0
}

// Parameterizedconstructorto initializewithaspecific value Class_type_one(float value)
 
{
a=value; // Initialize withtheprovidedvalue
}

// Function to returnthestored float value float get()
{
return a;
}

// Function to displaythe stored value void display()
{
cout <<a<< endl;
}
};

//classto be converted
// Class to receivetheconverted value class Class_type_two
{
float b; // Privatemembervariable to storetheconverted value

public:
// Overloading the assignment operatorto convert Class_type_one to Class_type_two void operator=(Class_type_one a_object)
{
b= a_object.get(); // Assignthe value fromClass_type_one'sobject to 'b'
}

// Function to displaythe stored value void display()
{
cout <<b << endl;
}
};

int main()
{
float input; // Variable to storeuser input
//cout << "Enterafloat value: "; // Prompt theuser cin >> input;// Read user input

Class_type_one obj1(input); // Create an object of Class_type_one and initialize with input value Class_type_two obj2; // Create an object of Class_type_two

obj2 = obj1; // Use theoverloaded '=' operatorto convert obj1 to obj2
 
obj1.display(); // Displaythevalue in obj1 (Class_type_one) obj2.display(); // Displaythevalue in obj2 (Class_type_two)

return 0; // Endtheprogram
}
```
## OUTPUT :
![image](https://github.com/user-attachments/assets/cb96073d-9340-4888-ab9d-30ba1dc7ed29)

## RESULT :

Thus, the C++ program for Class conversion that can be achieved by conversion function, which is done by the use of operator overloading, is created successfully.


