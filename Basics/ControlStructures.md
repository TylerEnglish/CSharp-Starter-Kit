# Control Structures in C#

Control structures are foundational elements in C#, directing the flow of program execution. They enable the incorporation of logic, decision-making, and repetition within your code. In this section, we will explore the primary control structures in C#.

## Conditional Statements

### `if` Statement
The `if` statement is used to execute a block of code only if a specified condition is true.

**Example:**
```csharp
int number = 5;
if (number > 0)
{
    Console.WriteLine("The number is positive.");
}

```

### `if-else` Statement
The `if-else` construct allows you to define an alternative block of code to be executed if the initial condition is false.

**Example:**
```csharp
int number = -3;
if (number > 0)
{
    Console.WriteLine("The number is positive.");
}
else
{
    Console.WriteLine("The number is negative.");
}

```

### `switch` Statement
The `switch` statement lets you select one of many code blocks to be executed, based on the value of a variable or an expression.

**Example:**
```csharp
int day = 4;
switch (day)
{
    case 1:
        Console.WriteLine("Monday");
        break;
    case 2:
        Console.WriteLine("Tuesday");
        break;
    case 3:
        Console.WriteLine("Wednesday");
        break;
    case 4:
        Console.WriteLine("Thursday");
        break;
    // ... Other cases ...
    default:
        Console.WriteLine("Invalid day");
        break;
}

```

## Looping Structures

### `for` Loop
The `for` loop is ideal for situations where you know beforehand how many times you wish to execute a statement or a block of statements.

**Example:**
```csharp
for (int i = 0; i < 5; i++)
{
    Console.WriteLine($"Iteration number: {i}");
}

```

### `while` Loop
The `while` loop repeatedly executes a block of code as long as a specified condition is true.

**Example:**
```csharp
int i = 0;
while (i < 5)
{
    Console.WriteLine($"Iteration number: {i}");
    i++;
}

```

### `do-while` Loop
Similar to the `while` loop, but the `do-while` loop tests the condition at the end of the loop, ensuring that the loop body is executed at least once.

**Example:**
```csharp
int i = 0;
do
{
    Console.WriteLine($"Iteration number: {i}");
    i++;
} while (i < 5);

```

### `foreach` Loop
The `foreach` loop is used to iterate over elements in a collection (e.g., an array or a list).

**Example:**
```csharp
string[] fruits = { "apple", "banana", "cherry" };
foreach (string fruit in fruits)
{
    Console.WriteLine(fruit);
}

```

## Jump Statements

### `break` Statement
Used to exit from a loop or a `switch` statement.

**Example:**
```csharp
for (int i = 0; i < 10; i++)
{
    if (i == 5)
    {
        break;
    }
    Console.WriteLine(i);
}

```

### `continue` Statement
Skips the current iteration in a loop and continues with the next iteration.

**Example:**
```csharp
for (int i = 0; i < 10; i++)
{
    if (i == 5)
    {
        continue;
    }
    Console.WriteLine(i);
}

```

## Conclusion

Control structures form the backbone of algorithmic logic in C#. By understanding and effectively using them, you can craft complex and efficient code structures.

[⬅️ Previous Lesson: Variables & Operators](./VariablesAndOperators.md) | [⬆️ Back to Table of Contents](../README.md) | [➡️ Next Lesson: Methods](./Methods.md)
