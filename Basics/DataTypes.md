# C# Data Types

In C#, as with many programming languages, data types define the nature of data that can be stored in a given variable. Understanding these is crucial to effective programming.

## Basic Types

### Integral Types

- **byte**: 8-bit unsigned integer (0 to 255).
- **sbyte**: 8-bit signed integer (-128 to 127).
- **int**: 32-bit signed integer (-2,147,483,648 to 2,147,483,647).
- **uint**: 32-bit unsigned integer (0 to 4,294,967,295).
- **short**: 16-bit signed integer (-32,768 to 32,767).
- **ushort**: 16-bit unsigned integer (0 to 65,535).
- **long**: 64-bit signed integer.
- **ulong**: 64-bit unsigned integer.

### Floating Point Types

- **float**: 32-bit single-precision floating-point number.
- **double**: 64-bit double-precision floating-point number.

### Decimal Type

- **decimal**: 128-bit precise decimal values, suitable for financial and monetary calculations.

### Boolean Type

- **bool**: Represents truth values, either `true` or `false`.

### Character Type

- **char**: Represents a single 16-bit Unicode character.

## Nullable Types

In C#, data types can be made nullable using the `?` modifier. This allows them to represent the usual range of values plus an additional `null`.

Example:
```csharp
int? nullableInt = null;
```

## Conclusion

Grasping the different data types is foundational for your journey into C#. As you delve deeper into the language, you'll encounter more complex types and structures.

[⬅️ Back to Table of Contents](../README.md) | [➡️ Proceed to Next Lesson: Variables & Operators](./VariablesAndOperators.md)

---

This `DataTypes.md` file offers a succinct breakdown of C#'s fundamental data types. As you progress through the Starter Kit, you'll find that subsequent documents, such as `VariablesAndOperators.md`, `ControlStructures.md`, and others, delve into increasingly intricate C# concepts.
