# My Coding Notebook

## Table of Contents 
- [Flutter Notes](#flutter-notes)
  - [What is Flutter](#what-is-flutter)
  - [KeyTerms and Definitions](#key-terms-and-definitions)
  - [Layout and Desgin Widgets](layout-and-desgin-widgets)
  - [Definition with Structures](#flutter-definition-with-structures)
- [Code Definition](#code-definition)
- [Notebook Style Guide](#markdown-style-guide-for-coding-notebooks)

- ## Flutter Notes

- ### What is flutter?
  - Definition: A framework made by Google for building apps that work on web,Android, and iOS with one codebase.
- Why is it useful?less money, less time, less work

---

### Key Terms and Definitions

| Term             | Definition                                      | Example / Notes                          |
|------------------|--------------------------------------------------|-------------------------------------------|
| Widget           | Basic building block of a flutter app.           |   Text,Image,Container,Column             |
| MaterialApp      | The root of the app. Sets up routes and themes   |   Found in main.dart                      |
| Scaffold         | Provides basic visual layout- like a header, body|   Each screen uses it                     |
| StatelessWidget  | A widget that doesn't change                     |   Most pf the screen files                |
| StatefulWidget   | A widget that can change over time               |   Used in MyHomePage                      |
| Navigator        | Manages screenn transitions                      |   Navigator.pushNamed(cont, '/page2");    |
| AppBar           | Top navigation bar                               |   Title of each page appears here         |
| Column           | vertical layout                                  |   Format of layout                        |
| Row              | horizontal layout                                |   Format of layout                        |
| Container        | wraps content with padding, margin,or color      |   Packages code and dependencies          |
| Named Routes     | Predefined paths to navigate between screens     |   '/','/page2','/page3',etc.              |
| Image.network    | displays images from a URL                       |    Images,text                            | 
| main()           | The function that runs the app                   |    Found in main.dart                     |



### Layout and Design Widgets
- How do you center a widget?
- How do you align something to the left or right?
- What widget adds space around content?


##Flutter Definition with structure
| Term | Definition and Description | Base Structure | Real Life Example | App Example |
|------|----------------------------|----------------|-------------------|-------------|
| Main() | A function that runs when your app starts. It tells Flutter what app to show. | `void main() => runApp(MyApp());` | starting a car | void main() => runApp(MyPortfolioApp()); |
| Material App | The widget that sets up your whole app’s look and navigation. | `MaterialApp(...)` | Front Cover |  return MaterialApp(debugShowCheckedModeBanner: false,title: 'TSA Portfolio',theme: ThemeData( |
| Scaffold | A widget that gives you the basic layout: background, navigation bar, floating button, etc. | `Scaffold(...)` | Desgin for a billboard | return Scaffold(body: Column(mainAxisAlignment: MainAxisAlignment.start,children: [ |
| Column | A widget that holds and displays your content in a straight line from top to bottom. | `Column(...)` | stacks |  body: Column(
 mainAxisAlignment: MainAxisAlignment.start,children: [ |
| Row | A widget that shows things side-by-side. | `Row(...)` | arrows for a wiki page | child: Row(children: [ |
| Container | A box that holds other widgets. You can add color, padding, borders, or size. | `Container(...)` | Shelves | return Container(margin:constEdgeInsets.symmetric (vertical: 8, horizontal: 16),padding: const EdgeInsets.all(12),decoration: BoxDecoration |
| Text | A widget to display text on the screen. | `Text('Hello')` | Documents |  const Text('HI EVERYONE,\nWelcome to the', |
| Image.network | A widget to show an image using a link from the internet. | `Image.network('https://...')` | PreView | child: Image.network('https://placedog.net/640/480?random', |
| ElevatedButton | A clickable button that floats above content. You choose what happens when it's clicked. | `ElevatedButton(onPressed: ..., child: ...)` | Button |  ElevatedButton(
onPressed: () => Navigator.pushNamed(context, '/showcase'),child: const Text('Next') |
|      | The code that gets run when a button is tapped or something happens. | `onPressed: () => doSomething()` |  |  |
| StatelessWidget | A class that creates widgets that never change. Good for static screens. | `class HomeScreen extends StatelessWidget` |  | HomePage |
| SatefulWidget | A class for widgets that can change while the app is running. | `class MyWidget extends StatefulWidget` | a ball | version 1.0 |
| Navigator | Lets you move from one screen to another using route names. | `Navigator.pushNamed(context, '/about')` |  |  |
| Padding | Makes space around a widget inside its container. | `Padding(padding: EdgeInsets.all(8.0), child: ...)` | make space | add containers |
| Center | Aligns content in the center of the screen or container. | `Center(child: ...)` | Paintings | Welcome App |
| Wrap | Automatically puts widgets onto a new line when there's no space. | `Wrap(children: [...])` |  |  
| @override | This marks a method as one that’s replacing a method in a parent class. | `@override` |  |  
| Build | The special function in every widget that describes what gets drawn on the screen. | `Widget build(BuildContext context) {...}` |  |  |
|      | Required in every widget class to describe what to show. | `build` |  |  |
|      | A variable that helps the widget know where it is and lets it communicate with the app. | `BuildContext context` |  |  |
|      | A keyword used to pass a value to the parent widget. | `super.key` |  |  |
|      | A keyword that means the value won't change and is set once. | `const` |  |  |


---
## Code Definition

| Term | Definition | Base Structure / Syntax | Real Life Example | App Example |
|------|------------|--------------------------|-------------------|-------------|
|Variable| A named container used to store a value that may change. | `var x = 5;` | Goals in soccer |
|Constant| A fixed value that cannot change once set. | `const PI = 3.14;` | File for a video |
|Data Type| The kind of value a variable holds, like numbers or text. | `int`, `String`, `bool` | Your age |
|String| A sequence of characters used to represent words or text. | `"Hello World"` | Messages | Title of the text |
|Integer| Whole number values. | `int age = 16;` | Streak | Notifications |
|Double| Number values with decimals. | `double age = 16.2;` | Smooth Movement | Progress | 
|Boolean| A value that can be true or false. | `bool isLoggedIn = false;` ||| 
|List| A collection of values in a specific order. | `List<String> names = [];` | Menu | Contact Log |
|Null| A special value that means “nothing.” | `String? name = null;` |||
|Function| A reusable block of code that performs an action. | `void sayHi() { print("Hi"); }` | Start a Car ||
|Parameter| The information passed into a function to change how it works. | `greet(String name)` | Shipping Address ||
|Return| The result a function gives back. | `return total;` | Confirmation Code | X to interact |
|Scope| Where a variable or function can be used. | (No set syntax — concept-based) | Limitations | Import files |
|Class| Blueprint for creating objects with specific structure and behavior. | `class Dog {}` |||
|Object| A specific version of a class. | `Dog myDog = Dog();` |  ||
|Property| A variable that belongs to a class/object. | `String name;` |
|Method| A function that belongs to a class. | `void bark() {}` |
|Constructor| A special function used to set up a class when it’s created. | `Dog(this.name);` |
|Abstraction| Hiding the inner workings of code so users only interact with what they need. | (Concept — not specific code) |
|Override| Changing how a built-in or inherited function behaves. | `@override` |
|Void| A function that does not return a value. | `void printMessage() {}` | 
|Scanner| creates a scanner object to take input from user | Scanner in = new Scanner(system.in) | | |
|Import Scanner| gives access to Scanner class, required at top to use Scanner| import java.util.Scanner; | | |
|Print statement| prints the content in the parenthesis   | | | |
|nextLine| reads in a STring from the user   | String str = input.nextLine(); | | |
|nextInt| reads in an int from the user   | int num = input.nextInt(); | | |
|nextDouble| reads in double(decimal) from the user   | double myDouble = input.nextDouble(); | | |
|nextBoolean| reads in Boolean(true/false) from the user   | boolean bool = input.nextBoolean(); | | |
|Arithmetic operaters| - * / %   | modulus,returns the reminder from dividing | | |
|Compound operaters| applies the result to the variable   | += -= *= /= %= ++ (adds 1) | | |
|Overloaded method/function or constructor| Uses the same name, but has different parameters | Pizza(), Pizza(String toppings) 2 constructors, first is a default cheese pizza, 2nd has 1 toppings| | |


## Markdown Style Guide for Coding Notebooks

Follow this guide to keep your coding notebook **clear, consistent, and professional**.  
This ensures your notes are easy for you (and others) to read later.

---

## 🔹 Headings
**When to use:** Organize your notebook into sections (like days, topics, or projects).  
- `#` for the notebook title (use once at the top).  
- `##` for each day or major topic.  
- `###` for subsections (like "Notes", "Practice", "Reflections").  

✅ Example:


# My Coding Notebook
## Day 1
### Notes
### Practice

🔡 Text Formatting
When to use: Highlight important ideas or add emphasis.

Use bold for key terms or definitions.

Use italic for emphasis or side comments.

Use inline code for keywords, functions, or commands.

 

✅ Example:

**Class** = a blueprint for objects  
*Remember:* always test your code  
Use `System.out.println()` to print

 

💻 Code Blocks
When to use: Anytime you write multiple lines of code.

Inline code for short snippets.

Fenced code blocks with language for full examples.

✅ Example:

```java
public class Hello {
    public static void main(String[] args) {
        System.out.println("Hello World!");
    }
}
```

🧾 Lists
When to use: Organize steps, notes, or key points.

Numbered lists for sequences or steps.

Bulleted lists for unordered ideas.

✅ Example:

1. Define the class
2. Write the main method
3. Test your program

Variables
- Loops
- Conditionals
 

✅ Checklists
When to use: Track progress on assignments or tasks.

✅ Example:

[x] Complete coding warm-up
- [ ] Finish project draft
- [ ] Reflect on learning

 

➡️ Blockquotes
When to use: Call out notes, reminders, or teacher comments.

✅ Example:

> 💡 Remember: Loops repeat code until a condition is false.

 

📊 Tables
When to use: Compare values, track progress, or organize data neatly.

✅ Example:

| Task        | Status   | Notes          |
|-------------|----------|----------------|
| Homework 1  | Done ✅  | Submitted      |
| Homework 2  | Pending  | Needs review   |

 

🔗 Links & Images
When to use: Add references, resources, or visuals.

✅ Example:

[Java Docs](https://docs.oracle.com/javase/8/docs/api/)  
![Markdown Logo](https://upload.wikimedia.org/wikipedia/commons/4/48/Markdown-mark.svg)

 

📂 Collapsible Sections
When to use: Hide solutions, extended notes, or extra details.

✅ Example:

<details>
  <summary>Click to reveal solution</summary>
  
System.out.println("Answer: 42");

</details>

 

📝 Footnotes
When to use: Add references or side notes without cluttering the page.

✅ Example:

This concept is related to object-oriented programming.[^1]

[^1]: See "Objects and Classes" in your textbook.

 

🎯 Style Rules
Consistency matters more than creativity

Always use headings to structure your notes.

Always use code blocks for multi-line code.

Clarity first

Bold key terms.

Use lists instead of long sentences when outlining steps.

Professional tone

Don’t mix casual notes with formal work in the same section.

Use blockquotes for reflections or teacher feedback.

Track your learning

Use checklists to mark what’s done.

Use collapsible sections if you want to hide answers until review time.

 

✅ Bottom Line:

Headings = Structure

Bold/Italic = Emphasis

Code blocks = Code

Lists = Steps/Ideas

Tables = Organization

Checklists = Progress

Blockquotes = Notes/Tips

Collapsible = Hide/Show detail

Keep it simple, consistent, and clear.
