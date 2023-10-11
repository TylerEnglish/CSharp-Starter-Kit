# Methods in C#

Methods in C# provide a way to bundle one or more statements into a single, callable unit. They are crucial for code organization, reusability, and separation of concerns.

## Why Use Methods?

- **Modularity**: Decompose a complex program into smaller, manageable units.
- **Reusability**: Define once, use repeatedly.
- **Readability**: Clearer, more concise code, especially for complex tasks.

## Defining a Method

Methods in C# have a defined signature, which includes a return type, a name, and optionally, parameters.

**Example:**
```csharp
public void SayHello()
{
    Console.WriteLine("Hello, World!");
}

```

## Returning Values from Methods

You can define methods to return values, allowing for computed results to be used elsewhere in your code.

**Example:**
```csharp
public int Multiply(int a, int b)
{
    return a * b;
}

```

## Parameters and Arguments

Methods can be parameterized to accept input values, enabling dynamic computation based on these inputs.

**Example:**
```csharp
public void DisplayGreeting(string name)
{
    Console.WriteLine($"Hello, {name}!");
}
// Usage: DisplayGreeting("Alice");

```

## Method Overloading

C# supports method overloading, allowing multiple methods in the same scope to have the same name as long as they have different parameters.

**Example:**
```csharp
public void DisplayInfo()
{
    Console.WriteLine("No information provided.");
}

public void DisplayInfo(string name)
{
    Console.WriteLine($"Name: {name}");
}

public void DisplayInfo(string name, int age)
{
    Console.WriteLine($"Name: {name}, Age: {age}");
}

```

## Default and Named Arguments

C# methods support default values for parameters and also allow for arguments to be passed by name, enhancing flexibility.

**Example:**
```csharp
public void CreateProfile(string name, int age = 30)
{
    Console.WriteLine($"Name: {name}, Age: {age}");
}
// Usage: CreateProfile(name: "Bob");
// Usage: CreateProfile(name: "Alice", age: 25);

```

## Recursive Methods

A method in C# can call itself, a feature that is particularly useful for tasks like factorial computation or tree traversal.

**Example:**
```csharp
public int Factorial(int n)
{
    if (n == 1)
        return 1;
    return n * Factorial(n - 1);
}
// Usage: int result = Factorial(5);  // result is 120

```

## Conclusion

Methods play a fundamental role in structuring C# programs, making them more maintainable, organized, and efficient. As you deepen your C# knowledge, you'll discover even more ways to leverage methods for sophisticated programming patterns.

[⬅️ Previous Lesson: Control Structures](./ControlStructures.md) | [⬆️ Back to Table of Contents](../README.md) | [➡️ Next Lesson: Classes & Objects](./ClassesAndObjects.md)
