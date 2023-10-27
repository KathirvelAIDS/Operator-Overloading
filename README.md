# Operator-Overloading

## Aim:
 To write a C# program to pass values through constructors(default and parameterized) and also overload equal operators by checking whether objects are equal using operator overloading. 
 
  
  ##Algorithm:
```
Step 1:
Create a class operator

Step 2:
Pass values through the constructor

Step 3:
return the bool operator, (==) and (!=)

Step 4:
create a object to store the return object

Step 5:
print the program
```
 
Program:
```
NAME:KATHIRVEL.
REG NO:212221230047
```
```
using System;
namespace ConsoleApp8
{
   class example
   {
       public int length;
       public example()
       {
           length = 10;
       }
       public example(int i)
       {
           length = i;
       }
       public static bool operator ==(example obj1, example obj2)
       {
           return obj1.Equals(obj2);
       }
       public static bool operator !=(example obj1, example obj2)
       {
           return !obj1.Equals(obj2);
       }
       public static void Main()
       {
           example e1 = new example();
           example e2 = new example(20);
           example e3 = new example();
           example e4 = e3;
           if (e3 == e4)
           {
               Console.WriteLine("Equal");
           }
           else if (e3 != e4)
           {
               Console.WriteLine("Not equal");
           }
       }
   }
}
```

 
 
 ##Output:
 
 ![image](https://github.com/KathirvelAIDS/Operator-Overloading/assets/94911373/d75d38c8-bc22-4b3c-8d59-01951ffffb1b)

 ##Result:
Thus the C# program to find the volume of a box using operator overloading is implemented successfully
