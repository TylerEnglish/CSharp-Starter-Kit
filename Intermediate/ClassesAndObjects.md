# Classes and Objects in C#

Classes and objects are the cornerstone of object-oriented programming (OOP) in C#. A class serves as a blueprint for creating objects, encapsulating data, and defining methods to interact with that data.

## Introduction to Classes

Classes in C# typically reside within namespaces, providing organization in larger projects.

**Example:**
```csharp
namespace MyApplication.Models
{
    public class Person
    {
        public string Name { get; set; }
        public int Age { get; set; }
    }
}

```


## Creating Objects (Instances)

Objects represent instances of a class, brought to life using the `new` keyword.

**Example:**
```csharp
Person person1 = new Person();
person1.Name = "Alice";
person1.Age = 30;

```


## Class Members

### Properties

Properties represent a class's data. They can be thought of as smart variables, giving more control over the data they hold through get and set accessors.

**Example:**
```csharp
public string Name { get; set; }
public int Age { get; private set; }

```


### Methods

Methods define actions or behaviors that a class can perform.

**Example:**
```csharp
public void IntroduceYourself()
{
    Console.WriteLine($"Hello, my name is {Name} and I am {Age} years old.");
}

```


## Constructors

Constructors are unique methods within a class responsible for initializing object state. They're called when an object is instantiated.

**Example:**
```csharp
public Person()
{
    Name = "Unknown";
    Age = 0;
}

public Person(string name, int age)
{
    Name = name;
    Age = age;
}

```


## The `this` Keyword

In C#, the `this` keyword is a reference to the current instance of a class. It's often used to distinguish between class members and method parameters.

**Example:**
```csharp
public void SetData(string Name, int Age)
{
    this.Name = Name; // Differentiates class member from method parameter
    this.Age = Age;
}

```


## Access Modifiers

Access modifiers like `public`, `private`, `protected`, and `internal` determine the accessibility and visibility of class members.

**Example:**
```csharp
public class SampleClass
{
    public string PublicString = "I'm accessible anywhere!";
    private string PrivateString = "I'm only accessible within this class.";
    protected string ProtectedString = "I'm accessible within this class and derived classes.";
    internal string InternalString = "I'm accessible within this assembly.";
}

```


## Conclusion

With a grasp of classes and objects, you're better equipped to understand the essence of OOP in C#. They enable you to model real-world entities, paving the way for robust and intuitive software design.

[⬅️ Previous Lesson: Methods](../Methods.md) | [⬆️ Back to Table of Contents](../README.md) | [➡️ Next Lesson: OOP Concepts](./OOPConcepts.md)
