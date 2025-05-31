# C++ COMPOSITION VS. INHERITANCE

## PROGRAM STATEMENT :

To write a CPP program to demonstrate on the object composition (use character data).

## ALGORITHM:  

1.	Start the program.
2.	Define a class A that has a character variable and a constructor to initialize it, along with a method to display its value.
3.	Define a class B that contains an object of class A and uses an initializer list to initialize it through B's constructor. Include a display method to show the value of A's object.
4.	In the main function, read a character input, create an object of class B with this input, and call the displa’y method.
5.	End the program.

## PROGRAM:
```
#include <iostream> #include <string> usingnamespacestd;

// Simple class class A {
char a; // Member variable to storethestring

public:
// Constructorthat initializes thestring 'a' A(char str)
{
a = str;
cout << "Constructor A(char a) is invoked" << endl;
}

//Method to displaythestringstored in 'a' void display()
{
cout << "Data in memberobject of class A in class B = " << a << endl;
}
};

// Complexclass class B {
 
AobjA; // Object of class A as amember of class B

public:
// Constructor that initializes the object 'objA' of class A B(charstr):objA(str) // Usinginitializer list to initialize objA
{
cout << "Data in object ofclass B = " << str << endl;
}

// Method to displaydata fromobject of class A void display()
{
objA.display();
}
};

// Driver code int main()
{
char input;
//cout << "Enterastring: "; cin >> input;

B objB(input); // Create an object of class B with the input string objB.display(); // Displaydata in objBand its composed object objA

return 0;
}
```
## OUTPUT :
![image](https://github.com/user-attachments/assets/1f8c3e0a-187a-4681-a9ad-3df7c0f2373d)

## RESULT :

Thus, the C++ program to demonstrate on the object composition is created successfully.


