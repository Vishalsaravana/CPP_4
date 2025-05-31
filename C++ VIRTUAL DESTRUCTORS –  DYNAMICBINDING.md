# C++ VIRTUAL FUNCTIONS – THIS POINTER

## PROGRAM STATEMENT :

To write a CPP program to override the print() function in the base class with the print() function in the child class using the concept of virtual functions.

## ALGORITHM:  

1.	Start the program.
2.	Define a base class with a virtual print method that outputs "Base class".
3.	Define a derived class that inherits from base and overrides the print method to read and display a string.
4.	In the main function, create a pointer of type base and an object of type derived.
5.	Assign the address of the derived object to the base pointer and call the print method using the pointer.
6.	End the program.

## PROGRAM:
```
#include<iostream> using namespace std; class base
{
public:
virtualvoidprint()
{
cout<<"Base class";
}
};
class derived:public base
{
public: string str; voidprint()
{
cin>>str; cout<<str<<endl;;
}
};
int main()
{
base*bptr;
 
derived d; bptr=&d; bptr->print();
}
```
## OUTPUT :
![image](https://github.com/user-attachments/assets/918663a9-653f-4028-a755-0fddde872e0f)

## RESULT :

Thus, the C++ program to override the print() function in the base class with the print() function in the child class using the concept of virtual functions is created successfully.
 


