# Objects And Its Representation in Js

## Objects:
Objects, in JavaScript, are the most important data type and form the building blocks for modern JavaScript. These objects are quite different from JavaScript’s primitive data types (Number, String, Boolean, null, undefined, and symbol) in the sense that these primitive data types all store a single value each .

Objects are more complex and each object may contain any combination of these primitive data-types as well as reference data-types.
An object is a reference data type. Variables that are assigned a reference value are given a reference or a pointer to that value. That reference or pointer points to the location in memory where the object is stored. The variables don’t actually store the value.
Loosely speaking, objects in JavaScript may be defined as an unordered collection of related data, of primitive or reference types, in the form of “key: value” pairs. These keys can be variables or functions and are called properties and methods, respectively, in the context of an object.

An object can be created with figure brackets {…} with an optional list of properties. A property is a “key: value” pair, where a key is a string or a symbol (also called a “property name”), and the value can be anything including numbers, strings, booleans, functions, arrays, or even other objects.

## Creating Objects:

In JavaScript, Objects can be created using two different methodologies namely Literal Form and Constructed Form.

**Literal Form:** The literal form uses the construction of object literals that can be said as a collection of key-value pairs enclosed within a pair of curly braces.

**Constructed Form:** The Constructed form uses either an object constructor function or the new keyword to create an empty object ad then adds properties to the object one by one. 
&nbsp;   **Object Constructor Function:** In this methodology, the user creates an explicit function to take required values as parameters and assign them as the properties of the desired object.
&nbsp;   **Using New Keyword:** This methodology uses the New keyword in front of any constructor method or any built-in constructor method ( such as Object, Date, String, etc) and creates a new instance of the following object by mounting it on memory.

## Build-in Objects:
JavaScript consists of a bunch of Built-In Objects, the following list explores most of them. Although these built-ins have the appearance of being actual types or classes like in any other OOP, in JavaScript these are only functions that can be used as constructors to create objects of the particular sub-type.

-String
-Number
-Boolean
-Object
-Function
-Array
-Date
-RegExp
-Error

## Content of Objects:
JavaScript objects consist of a set of key-value pairs, which are known as Properties. All Properties are named in JavaScript objects and the key part represents the Property name, while the value part represents the property Value. The Property Value can be of the primitive data type or an object or even a function. The property can also be globally accessible in spite of being owned by an object.

## Objects properties:

A JavaScript object has properties associated with it. A property of an object can be explained as a variable that is attached to the object. Object properties are basically the same as ordinary JavaScript variables, except for the attachment to objects. The properties of an object define the characteristics of the object. You access the properties of an object with a simple dot-notation:

objectName.propertyName

Like all JavaScript variables, both the object name (which could be a normal variable) and property name are case sensitive. You can define a property by assigning it a value.
Properties of JavaScript objects can also be accessed or set using a bracket notation. Objects are sometimes called associative arrays, since each property is associated with a string value that can be used to access it. 

Inherited properties of an object are those properties that have been inherited from the object’s prototype, as opposed to being defined for the object itself, which is known as the object’s Own property. To verify if a property is an object’s Own property, we can use the hasOwnProperty method. Property Attributes Data properties in JavaScript have four attributes.



An object property name can be any valid JavaScript string, or anything that can be converted to a string, including the empty string. However, any property name that is not a valid JavaScript identifier (for example, a property name that has a space or a hyphen, or that starts with a number) can only be accessed using the square bracket notation. This notation is also very useful when property names are to be dynamically determined (when the property name is not determined until runtime).  You can also access properties by using a string value that is stored in a variable:


You can use the bracket notation with for...in to iterate over all the enumerable properties of an object. To illustrate how this works, the following function displays the properties of the object when you pass the object and the object's name as arguments to the function:


## Important Points:
Date values can only be created with their constructed object form, as they have no literal form.
Objects, Arrays, Functions, and RegExps (regular expressions) are all objects regardless of their creation methodologies i.e. whether the literal or constructed form was used to create them.
The constructed form may offer more customization while creating an object, this is the sole advantage over using the literal form.

