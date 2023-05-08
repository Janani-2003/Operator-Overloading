# Operator-Overloading

## Aim:
 To write a C# program to pass values through constructors(default and parameterized) and also overload equal operators by checking whether objects are equal using operator overloading. 
 
 ## Algorithm:
### Step 1:
Create a class for operator overloading

### Step 2:
Get inputs for length,breadth from the user in overloading function.

### Step 3:
Compare the inputs such as length and breadth.

### Step 4:
Using equal to(==) and not equal to(!=) operator we can compare the inputs.

### Step 5:
After that print the result.
 
 
 ## Program:
 ```
 Developed by : JANANI R
 Register number : 212221230039
 ```
 ```
 using System;
    class program
    {
        public program(int p1, int p2)
        {
            Console.WriteLine(p1 * p2);
        }
        public program(int p1)
        {
        Console.WriteLine(p1 * 1);
        }
        public static bool operator == (program p1, program p2)
        {
            return p1.Equals(p2);
        }
        public static bool operator != (program p1, program p2)
        {
            return !p1.Equals(p2);
        }

    }
    class Example
    {
        public static void Main()
        {
            program p1 = new program(10,20);
            program p2 = new program(10);
            p1 = p2;
            if(p1==p2)
            {
                Console.WriteLine("Objects are equal");
            }
            else
            {
                Console.WriteLine("Objects are not equal");
            }
        }
    }


 ```
 
 ## Output:
 ![Screenshot 2023-05-08 145423](https://user-images.githubusercontent.com/94288340/236788599-1fdb31c0-ac42-4055-8703-8d05cfcd55a3.png)
 
 ## Result:
Thus the C# program to find the volume of a box using operator overloading is implemented successfully.
