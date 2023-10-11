# Object-Oriented Programming (OOP) Concepts in C#

Object-Oriented Programming (OOP) is a paradigm that uses "objects" and classes for organizing code. It revolves around several core concepts: Encapsulation, Inheritance, Polymorphism, and Abstraction. C# being an object-oriented language, embraces these concepts, allowing developers to create modular and scalable applications.

## Encapsulation

Encapsulation refers to bundling data (attributes) and methods (functions) into a single unit, or class. It also involves restricting direct access to some of the object's components, which can be achieved using access modifiers.

**Example:**
```csharp
public class BankAccount
{
    private double _balance;

    public BankAccount(double initialBalance)
    {
        _balance = initialBalance;
    }

    public double Balance 
    { 
        get { return _balance; }
    }

    public void Deposit(double amount)
    {
        _balance += amount;
    }

    public bool Withdraw(double amount)
    {
        if (amount <= _balance)
        {
            _balance -= amount;
            return true;
        }
        return false;
    }
}

```

## Inheritance

Inheritance allows a class (child or derived class) to inherit attributes and methods from another class (parent or base class). This promotes code reusability and establishes a relationship between the parent and child classes.

**Example:**
```csharp
public class Vehicle
{
    public string Brand { get; set; }

    public void Honk()
    {
        Console.WriteLine("Honk! Honk!");
    }
}

public class Car : Vehicle
{
    public int Wheels = 4;
}

```

## Polymorphism

Polymorphism, meaning "many shapes," is the ability of different classes to be treated as instances of the same class through inheritance. This can be achieved in C# using method overriding, virtual functions, and abstract classes.

**Example:**
```csharp
public class Animal
{
    public virtual void Speak()
    {
        Console.WriteLine("The animal makes a sound.");
    }
}

public class Dog : Animal
{
    public override void Speak()
    {
        Console.WriteLine("The dog barks.");
    }
}

public class Cat : Animal
{
    public override void Speak()
    {
        Console.WriteLine("The cat meows.");
    }
}

```

## Abstraction

Abstraction means using simple classes to represent complex systems by hiding intricate details and showing only the essential features. This is achieved in C# using interfaces and abstract classes.

**Example:**
```csharp
public abstract class Shape
{
    public abstract double Area();

    public abstract double Perimeter();
}

public class Circle : Shape
{
    public double Radius { get; set; }

    public override double Area()
    {
        return Math.PI * Radius * Radius;
    }

    public override double Perimeter()
    {
        return 2 * Math.PI * Radius;
    }
}

public class Rectangle : Shape
{
    public double Width { get; set; }
    public double Height { get; set; }

    public override double Area()
    {
        return Width * Height;
    }

    public override double Perimeter()
    {
        return 2 * (Width + Height);
    }
}

```

## Conclusion

Mastering the concepts of OOP is crucial for any C# developer. Not only does it provide a way to structure and organize code effectively, but it also paves the way for advanced programming techniques and design patterns.

[⬅️ Previous Lesson: Classes & Objects](./ClassesAndObjects.md) | [➡️ Back to Table of Contents](../README.md)
