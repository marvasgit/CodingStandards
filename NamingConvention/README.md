# General Naming Guidelines

## Table of Content

1. [Applications](Applications.md)
1. [ProjectFolders](ProjectFolders.md)
1. [Files](Files.md)
1. [Assemblies](Assemblies.md)
1. [Namespaces](Namespaces.md)
1. [Interfaces](Interfaces.md)
1. [Classes](Classes.md)
1. [Variables](Variables.md)
1. [Types](Types.md)
1. [Boolean](Boolean.md)
1. [Enumerations](Enumerations.md)
1. [Constants](Constants.md)
1. [Methods](Methods.md)
1. [MethodParameters](MethodParameters.md)
1. [SpeacialVariables](SpeacialVariables.md)

**Always use English**
  
***Use Intention-Revealing Names***

  - What does this class do?
  - What is the intent of this variable?
  - What is this variable / class used for?

**Whether a name is meaningful or not depends on its context (its enclosing type)**

 * Examples of meaningful names:
        * [x] Generate() in the class LabyrinthGenerator
        * [x] Find(string fileName) in the class FileFinder
        * [x] Deposit(decimal amount) in the class Account
* Examples of meaningless names:
  * [x] Generate() in the class Program
  * [x] Find(string name) in the class Program

* Often mistate is to use “fake” meaningful names that are in fact meaningless

* Yes, **Topic6Exercise12** indicates that this is solution to exercise 12, but what is it about?
  * Proper naming doens't require a validation of what exactly is variable for.
* Better naming:
* [x] MaximalNumbersSubsequence, MinimalTripAmount..

***

* Avoid hard-to-pronounce names or abbreviations
 **dtbgRegExPtrn** vs. **dateTimeBulgarianRegExPattern**
 , **scrpCnt** vs. **scriptsCount**

* Avoid using encodings
  * Example: ***nameString*** vs. ***name***

#### Good :

```C#
heavyCheckMark,
FactorialCalculator,
studentsCount,
Math.PI,
configFileName,
CreateReport
```

#### Bad

```C#
k,
k2,
k3,
junk,
f33,
KJJ,
button1,
variable,
temp,
tmp,
temp_var,
something,
someValue
```

## Bad naming examples

```c#
Topic6Exercise12,
LoopsExercise12,
Problem7,
OOPLecture_LastExercise
```

**Pick One Word per Concept**

**Solution Domain Names vs Problem Domain Names**
The clean code philosophy suggests using solution domain names such as the name of algorithms or the name of design patterns whenever needed, and use a problem domain name as the second choice.

For example, accountVisitor means a lot to a programmer who is familiar with the Visitor design pattern. A "JobQueue" definitely make more sense to a programmer.

**Make Meaningful Distinctions**
If there are two different things in the same scope, you might be tempted to change one name in an arbitrary way.

What is stored in cust, which is different from customer?

String cust;  
String customer;

## Names to Avoid

* Don't use numbers in the identifiers names
  * Example:

    ```C#
    PrintReport and PrintReport2
    ```

  * What is the difference?
  * Exceptions:
    * When the number is part of the name itself,e.g. **RS232Port**, **COM3**, **Win32APIFunctions**
* Don't use letters from other alphabet

**FindСтудентByName**, **DisplayΩ2Protein**

## Never Give Misleading Name

* Giving a misleading name is even worse than giving a totally unclear name
  * Example:
  * Consider a method that calculates the sum of all elements in an array
  * Its should be named **Sum** or **CalculateSum**
  * What about naming it **CalculateAverage** or **Max** or **CheckForNegativeNumber**?

## IT'S CRAZY, BUT BE CAREFUL WITH "COPY-PASTE"
