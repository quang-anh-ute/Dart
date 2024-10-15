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

### BloC
Bloc (Business Logic Component) is a state management pattern used in Flutter to separate presentation logic from business logic. It helps to manage and maintain the app state, making it easier to test, debug, and reuse code. It uses streams to emit new states and reacts to changes in the state.
https://www.youtube.com/watch?v=Ep6R7U9wa0U

### Provider
Provider is a wrapper around InheritedWidget (base class for widgets that efficiently propagate information down the tree) to make them easier to use and more reusable.

## JSON
JSON (JavaScript Object Notation) is a lightweight data interchange format that is easy for humans to read and write and easy for machines to parse and generate. In Flutter, JSON is used for transmitting data between the client and server, typically over an HTTP connection.

Flutter provides a number of libraries for working with JSON data, including the dart:convert library, which provides support for encoding and decoding JSON data.

To encode a Dart object to a JSON string, you can use the jsonEncode function from the dart:convert library. To decode a JSON string to a Dart object, you can use the jsonDecode function.

https://docs.flutter.dev/data-and-backend/serialization/json

## AnimationController
This class lets you perform tasks such as:

Play an animation forward or in reverse, or stop an animation.
Set the animation to a specific value.
Define the upperBound and lowerBound values of an animation.
Create a fling animation effect using a physics simulation.

## AnimatedBuilder
AnimatedBuilder is a widget in Flutter that allows you to build animations. It takes an Animation object and a builder function as input, and it returns a widget that is rebuilt whenever the animation changes. The builder function is called with the BuildContext and the animation object and it should return the widget that should be animated. This can be used to create complex animations with ease, without having to manage animation state or listen to animation events in the widget tree.

## AnimatedWidget
AnimatedWidget is a Flutter widget that takes an Animation object as an argument and automatically updates whenever the animation changes. This can be useful when you want to create animations that are tightly coupled to a widget, for example, to animate the size or color of a widget. With AnimatedWidget, you can encapsulate the animation logic into a single widget and reuse it throughout your app. This makes it easier to manage and maintain your animations, as the animation code is centralized and decoupled from the widget tree.

## Widget Testing
Widget testing in Flutter is the process of testing the behavior and appearance of individual widgets, in isolation from the rest of your app. It allows you to verify that a widget works correctly, displays the expected output, and behaves correctly in response to user interactions.

In Flutter, you can write widget tests using the flutter_test package, which provides a testing framework for writing and running widget tests. A widget test is similar to a unit test, but instead of testing individual functions, you test entire widgets. You can use the TestWidgetsFlutterBinding to run your widget tests and simulate user interactions, such as taps, scrolls, and other gestures.

The framework provides several utility functions to help you build and test widgets, such as pumpWidget, which allows you to pump a widget and its children into the widget tree and simulate a frame of animation, and find, which allows you to search the widget tree for a widget that matches specific criteria.

## Integration Testing
Integration tests in Flutter are tests that verify the behavior of your app as a whole, rather than individual widgets or functions. Integration tests allow you to test the interactions between different parts of your app and verify that the overall behavior of the app is correct.

In Flutter, you can write integration tests using the flutter_driver package, which provides a testing framework for writing and running integration tests. An integration test runs on a physical device or an emulator, and uses the FlutterDriver class to interact with the app and simulate user interactions, such as taps, scrolls, and gestures.

The framework provides several utility functions to help you interact with your app, such as tap, scroll, and enterText, which allow you to perform actions in your app and verify its behavior. You can also use waitFor, which allows you to wait for specific conditions to be met before continuing with the test.
