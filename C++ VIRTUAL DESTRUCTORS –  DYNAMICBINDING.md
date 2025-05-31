# C++ VIRTUAL DESTRUCTORS – DYNAMIC BINDING

## PROGRAM STATEMENT :

To write a CPP program to show how the override works using virtual functions and how it works without the virtual concept.

## ALGORITHM:  

1.	Start the program.
2.	Define a base class with two methods: disp (virtual) and disp1 (non-virtual), each reading a string input and printing a message.
3.	Define a derived class that inherits from base and overrides both disp and disp1 to read and print a different message.
4.	In the main function, create a pointer of type base and an object of type derived.
5.	Assign the address of the derived object to the base pointer.
6.	Use the pointer to call the disp method (virtual, bound at runtime) and disp1 method (non- virtual, bound at compile time).
7.	End the program.

## PROGRAM:
```
#include<iostream> using namespace std;

classbase{ public : stringstr;
virtualvoiddisp()
{
cin>>str;
cout<<str<<" Base Class Not overridden"<<endl;
}
void disp1()
{
cin>>str;
cout<<str<<" Base Class Not overridden"<<endl;
}
};

classderived: publicbase{ public:
string str2;
 
voiddisp()
{
cin>>str2;
cout<<str2<<" Derived Class Overridding"<<endl;
}

void disp1()
{
cin>>str2;
cout<<str2<<" Derived Class Overridding"<<endl;
}
};

int main()
{
//Base ClassPointer base *bptr;
//Derived Class Object derived d;
//AssignBase Class Pointerwith Derivedclass Object bptr = &d;

//Virtual function, binded at runtime bptr->disp();
//Non-virtual function, binded at compiletime bptr->disp1();

return 0;
}
```
## OUTPUT :
![image](https://github.com/user-attachments/assets/514259d5-3223-461d-b7f2-30f283e97cc1)


## RESULT :

Thus, the C++ program to show how the override works using virtual functions and how it works without the virtual concept is created successfully.
 
