# Recitation 3 - Implementing Classes

## Learning Outcomes

By the end of this activity, a student should be able to:
1. Implement a simple Java class
2. Implement constructors
3. implement accessor and mutator methods

## Introduction

This recitation requires that you to implement a Circle class.  This recitation is available on Github Classroom.  Click on the link in Blackboard to accept the assignment and clone the repo using IntelliJ.

## Implementing a Circle Class
A circle is an object that can be described by its location and radius.  Depending on the application, a circle may have other properties like color, line width, fill color, etc...  For the purpose of this recitation, it is sufficient to describe our circle using the location and radius.  As such, our Circle class must include three fields called x, y, and radius.  It should be noted that we could use the Point class that was developed in class; however, this will be the topic on the next recitation after we develop some concepts in this week's lectures.

Based on the information above, our class at a minimum will look like,

```java
/**
 * This class provides a simple Circle type that
 * creates and tracks instances of circles.
 *
 * @author (You Me)
 * @version (2018-02-05)
 */
public class Circle
{
    //instance variables
    private double x;
    private double y;
    private double radius;
}
```

## Implementing Constructors

Let's add a default constructor to this class that initializes the a new instance of Circle to x to 0, y to 0, and radius to 1.0.  In the template for Circle class below, you should see a skeleton implementation of the default constructor,

```java
/**
   * Defualt constructor that initializes an instance of Circle
   * to (0,0) with a radius of 1.0.
   */
  public Circle()
  {
      // TODO - replace this line with your code
  }
```

Add your code so that a new instance has its instance variable initialized to the values stated above.

## Overloading the Constructor

There are two more constructors in the template provided below for the Circle class.  Insert your code so that the constructors behave as described in their respective comment documentation. For the second constructor,

```java
/**
   * Constructor that initializes an instance of Circle to (0,0)
   * with a radius given by the parameter radius.
   * 
   * @param radius the radius of this circle.
   */
  public Circle(double radius)
  {
      // TODO - replace this line with your code
  }
```

add code to initialize instance variables x to 0, y to 0, and radius to the the value of radius given by the parameter.

For the third constructor,

```java
/**
   * Constructor that initializes an instance of Circle to (x,y)
   * with a radius given by the parameter radius.
   * 
   * @param x the location of the center of this circle along the x coordinate
   * @param y the location of the center of this circle along the y coordinate
   * @param radius the radius of this circle.
   */
  public Circle(double x, double y, double radius)
  {
      // TODO - replace this line with your code
  }
```
add code to initialize instance variables `x`, `y`, and `radius` to the value of the same name  parameters.

## Accessor Methods

Now, implement the three accessor methods `getRadius`, `getX`, and `getY` so that they return the appropriate information.  Each accessor method is documented in the template below.

## Mutator Methods

Now, implement the three mutator methods `setRadius`, `setX`, and `setY` so that they return the appropriate information.  Each mutator method is documented in the template below.

## Submit Code

Ensure that all constructors and methods work correctly by setting up a Graddle run configuration.  Your project comes with a test class that tests all your methods and constructors.  Once your test runs successfully, push your work to the repo.