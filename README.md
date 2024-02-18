# EX-1 Eligibility-for-Engineering-Admission
## Aim:
To write a C# program to check whether the student is eligibile for the engineering admission
## Algorithm:
### Step1: 
Create new class
### Step2: 
Initiate the variables for maths, physics and chemistry and get the value from the user.
### Step3:
Convert the values to integer values.
### Step4:
Calculate the sum of all three subjects and maths-physics total.
### Step5:
Check for the given criteria for eligibility using if-else statements.
### Step6:
Display whether the person is eligible for admission or not based on the given criteria.
### Step7:
Exit the Program.
## Program:
```
Name : G.Jayanth.
Ref No: 212221230030.
```

```
using System;

namespace exp1
{
    class Eligibility
    {
        static void Main(string[] args)
        {
            string name;
            int math, phy, chem;
            Console.Write("Enter your name:");
            name = Console.ReadLine();
            Console.Write("Enter Maths Marks:");
            math = Convert.ToInt32(Console.ReadLine());
            Console.Write("Enter Physics Marks:");
            phy = Convert.ToInt32(Console.ReadLine());
            Console.Write("Enter Chemistry Marks:");
            chem = Convert.ToInt32(Console.ReadLine());
            int Sum = math + phy + chem;
            int MPTot = math + phy;
            if (math >= 65 && phy >= 55 && chem >= 50)
            {
                if (Sum >= 180 || MPTot >= 140)
                {
                    Console.WriteLine(name + " is eligible for admission to an engineering course.");
                }
                else
                {
                    Console.WriteLine(name + " is not eligible for admission to an engineering course due to insufficient marks.");
                }
            }
            else
            {
                Console.WriteLine(name + " is not eligible for admission to an engineering course due to insufficient marks.");
            }
            Console.Read();
        }
    }
}

```
## Output:

<img width="929" alt="ex1 eligibility" src="https://github.com/JayanthYadav123/Eligibility-for-Engineering-Admission/assets/94836154/c39b409f-c022-40d6-8e50-fc4bcddcd5ca">

## Result:
Thus the above C# program to check the eligibility of engineering admission is successfully executed.

