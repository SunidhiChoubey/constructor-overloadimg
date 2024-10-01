# EXPERIMENT- 13
# constructor-overloadimg
## AIM- To study and implement Constructor Overloading
## Theory
Constructor Overloading in C++:
Multiple Constructors: A class can have multiple constructors with different parameter lists.
Different Parameters: Constructors must differ by number, type, or order of parameters.
Automatic Selection: The compiler selects the appropriate constructor based on provided arguments.
Flexible Initialization: Allows different ways to initialize objects.
Same Name: All overloaded constructors share the class name.
No Return Type: Overloaded constructors don't have a return type.
Advantages:
Flexibility: Enables object creation in various ways.
Ease of Use: Simplifies initialization with different data.
Readability: Clearly defines how objects can be created.
Rules:
Different Signatures: Each constructor must have unique parameters.
Same Name and No Return Type: All constructors follow these rules.
How It Works:
If no arguments are passed, the default constructor is called.
If arguments are passed, the matching constructor is invoked.

## Code
~~~
# include<iostream>
using namespace std;

class room
{
    private:
    double l,b;

    public:
    room()
    {
        l = 1.2;
        b = 2.3;
    }
    room(double len, double bre)
    {
        l = len;
        b = bre;
    }
    room(double len)
    {
        l = len;
        b = 4.5;
    }
    double area()
    {
        return l*b;
    }

};
int main()
{
    room r1,r2(6.7,7.8),r3(9.1);
    cout<<"No parameter passed: "<<endl;
    cout<<"Area: "<<r1.area()<<endl;
    cout<<"Two parameters passed: "<<endl;
    cout<<"Area: "<<r2.area()<<endl;
    cout<<"One parameter passed: "<<endl;
    cout<<"Area: "<<r3.area()<<endl;
}
~~~
## Output-
![](https://github.com/SunidhiChoubey/constructor-overloadimg/blob/main/Screenshot%202024-10-01%20011519.png)

## Conclusion-
we  learnt bout construction overloading
