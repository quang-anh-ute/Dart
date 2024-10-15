## Built-in Types
There are several built-in data types, including:

    int: used to store integers
    double: used to store floating-point numbers
    String: used to store text
    bool: used to store true or false values
    List: used to store ordered collections of objects
    Sets: used to store unordered collection of unique items
    Map: used to store unordered collections of key-value pairs
    Additionally, there are other complex data types like dynamic, var, and Object in Dart programming language which is used in Flutter.
https://dart.dev/language/built-in-types

https://dart.dev/language/collections

## Functions
Dart is a true object-oriented language, so even functions are objects and have a type, Function. This means that functions can be assigned to variables or passed as arguments to other functions. You can also call an instance of a Dart class as if it were a function.
https://javatpoint.com/dart-function

## Operators
Operators are symbols or keywords used to perform operations on values. There are several types of operators available in Flutter:

Arithmetic operators: used to perform mathematical operations like addition (+), subtraction (-), multiplication (*), division (/), and more.
Relational operators: used to compare values and return a boolean result (==, !=, >, <, >=, <=).
Logical operators: used to perform logical operations like AND (&&), OR (||), and NOT (!).
Assignment operators: used to assign values to variables (=, +=, -=, *=, /=, %=).
Ternary operator: a shorthand way of writing simple if-else statements (condition ? if_true : if_false).
These operators can be used to perform operations on values, variables, and expressions in Flutter.

## Control Flow Statements
In Dart, control flow statements are used to control the flow of execution of a program. The following are the main types of control flow statements in Dart:

if-else: used to conditionally execute code based on a boolean expression.
for loop: used to repeat a block of code a specific number of times.
while loop: used to repeat a block of code as long as a given condition is true.
do-while loop: similar to the while loop, but the block of code is executed at least once before the condition is evaluated.
switch-case: used to select one of several code blocks to execute based on a value.
break: used to exit a loop early.
continue: used to skip the current iteration of a loop and continue with the next one.
These control flow statements can be used to create complex logic and control the flow of execution in Dart programs.

## Stateless Widgets
Stateless widgets in Flutter are widgets that don’t maintain any mutable state. They are designed to be immutable and rebuild each time the framework needs to update the UI. They are suitable for static, unchanging views or simple animations. They can be created using the StatelessWidget class and have a single build method that returns a widget tree.
       
        https://api.flutter.dev/flutter/widgets/StatelessWidget-class.html
        https://medium.com/flutter/how-to-create-stateless-widgets-6f33931d859

## Stateful widgets
A stateful widget is dynamic: for example, it can change its appearance in response to events triggered by user interactions or when it receives data. Checkbox, Radio, Slider, InkWell, Form, and TextField are examples of stateful widgets.

        https://api.flutter.dev/flutter/widgets/StatefulWidget-class.html
        https://www.youtube.com/watch?v=p5dkB3Mrxdo

## State Management
State management in Flutter refers to the process of managing and updating the data or state of a Flutter application. In Flutter, the state of the widgets can change dynamically, for example, when a user interacts with the application. The state management techniques in Flutter include:

    Provider: a lightweight solution that allows widgets to access the state with minimal boilerplate code.
    BLoC (Business Logic Component): a state management technique that uses streams and reactive programming to manage the state.
Redux: a state management solution inspired by the Redux library in React.
InheritedWidget: a built-in widget that allows the state to be passed down the widget tree.
ScopedModel: a third-party state management solution that uses a centralized model to manage the state.

The choice of state management technique depends on the complexity and size of the project. For smaller projects, Provider or InheritedWidget may be sufficient, while larger projects may require a more robust solution like ScopedModel or Redux.
