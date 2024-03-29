---
title: "Unity Variable Data Types"
description: Basic data types in Unity
date: 2024-03-23T12:25:26-04:00
image: /post/C/variables.jpg
hidden: false
comments: false
draft: false
links:
  - title: Unity Docs
    description: Here is the scripting documentation for Unity.
    website: https://docs.unity3d.com/ScriptReference/index.html
    image: https://cdn.sanity.io/images/fuvbjjlp/production/2d61dff37585fcd78d7e407f4ba79cf89000d5c3-109x103.png
---

Hello, welcome to my first official post for my new blog.
Let's start with a basic breakdown of data types for Unity scripting. Think of it like a cheat sheet of sorts to check on now and then.

With C#, data types are used to define the type of data that a variable can hold. We're looking through Unity Engine specifically because it uses C# as its primary programming language. Here are some of the basic data types you’ll encounter when scripting. To get started with creating a script, right-click on the project window and click on Create -> C# script.

## Basic Data Types

### Integers

```
int score = 0;
```

An int or integer is a data type that holds a whole number, positive or negative. Important note is that ints cannot be decimals, only whole numbers here.

### Floats

```
float speed = 5.5f;
```

A float represents a floating-point number, the main difference between an int and a float is that floats can have decimal points. Append an ‘f’ at the end to signal to Unity that it is a float.

### Booleans

```
bool isJumping = false;
```

A bool or boolean represents a state that can be either true or false.

### Strings

```
string playerName = "Alex";
```

A string represents a sequence of characters. For Unity, you might use strings to store names, UI text, currency names or more.

## Advanced Data Types

### Colors

```
Color backgroundColor = Color.red;
```

The Color data type stores values for Red, Green, Blue, and Alpha (transparency).

### Arrays

```
int[] scores;
```

An array is a collection of variables of the same type. You can store multiple values in a single array variable. In Unity, you can add or remove entries of an array within the inspector. Remember, arrays will start with the data entry of 0, not 1.

### Lists

```
List<int> scores;
```

A List is similar to an array but with additional functionality such as adding and removing elements at runtime.

### Dictionaries

```
Dictionary<string, int> inventory;
```

A Dictionary is a collection of key-value pairs. For example, you might use a dictionary to store an inventory of items, where the item name is the key and the quantity is the value.

### Vector3

```
Vector3 playerPosition = new Vector3(0, 0, 0);
```

A Vector3 represents a three-dimensional vector, commonly used for positions, directions, and more in 3D space.

## Protection levels

### Public

```
public int score = 0;
```

Public data types are like open fields in your code. Any script when given a reference can access and modify the specified variable directly. You will also see any publicly defined variables within the inspector menu back in Unity.

### Private

```
private int score = 0;
```

Private data types are exclusive to the script they're declared in. Other scripts can't **directly** access them. One note is that an effect of a variable becoming private is that it will not appear in the inspector menu back in the Unity Editor.

These are just a few of the many different variables you will use when scripting in Unity. If you want a deeper dive into variable types with components, please use the official Unity documentation linked below.

Sources:
Unity Docs
