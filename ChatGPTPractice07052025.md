Explain to me as if I am brand new to C# coding five of the most useful formulas to use C# coding with three examples of each of the five formulas and an explanation of each of the five formulas. 

Sure! Since you're brand new to C# coding, I'll explain five of the most useful and common "formulas" (in programming, we usually call them constructs, statements, or syntax patterns) that you'll use often when coding in C#. These are tools to help you write logic, manage data, and control the flow of your program.

 1. Variable Declaration and Assignment
 What it does:
Variables let you store data in memory to use later. You "declare" a variable by giving it a type and a name, then you can assign it a value.

Syntax:
<dataType> <variableName> = <value>;

Examples:
int age = 25;                  // Stores an integer
string name = "Alice";         // Stores a text (string)
bool isLoggedIn = true;        // Stores a true/false value

Explanation:
This is the most basic and essential part of programming. Everything starts with storing data. You choose a type (int, string, bool, etc.), give it a name, and set a value.

 2. If-Else Statement (Decision Making)
 What it does:
Checks a condition and runs different code depending on whether it's true or false.
if (condition) {
    // do this if true
} else {
    // do this if false
}

Examples:
int age = 18;
if (age >= 18) {
    Console.WriteLine("You're an adult.");
} else {
    Console.WriteLine("You're a minor.");
}

bool isRaining = false;
if (isRaining) {
    Console.WriteLine("Take an umbrella!");
} else {
    Console.WriteLine("No umbrella needed.");
}

string password = "abc123";
if (password == "admin") {
    Console.WriteLine("Welcome, Admin.");
} else {
    Console.WriteLine("Access Denied.");
}

Explanation:
This is how your program makes decisions. It checks conditions and behaves differently based on the result. Super useful for things like login checks, input validation, and game logic.

3. For Loop (Repetition)

What it does:
Repeats a block of code a set number of times.

Syntax:

for (int i = 0; i < limit; i++) {
    // code to repeat
}

for (int i = 0; i < 5; i++) {
    Console.WriteLine(i);  // Prints 0 to 4
}

for (int i = 1; i <= 10; i++) {
    Console.WriteLine(i * i);  // Prints squares of numbers from 1 to 10
}

string[] colors = {"Red", "Green", "Blue"};
for (int i = 0; i < colors.Length; i++) {
    Console.WriteLine(colors[i]);
}

Explanation:

Loops are key for doing something many times. This is great for things like printing items in a list, counting, or doing math calculations repeatedly.

4. While Loop (Conditional Repetition)

What it does:

Repeats a block of code while a condition is true.

Syntax:

while (condition) {
    // code to repeat
}

Examples:

int count = 0;
while (count < 3) {
    Console.WriteLine("Hello!");
    count++;
}

int number = 5;
while (number > 0) {
    Console.WriteLine(number);
    number--;
}

bool keepGoing = true;
int input = 0;
while (keepGoing) {
    Console.WriteLine("Enter a number (0 to stop): ");
    input = Convert.ToInt32(Console.ReadLine());
    if (input == 0) {
        keepGoing = false;
    }
}

Explanation:

Use a while loop when you don’t know in advance how many times something will repeat — only that it depends on a condition.

5. Method (Function) Declaration and Calling

What it does:

Wraps code into a reusable block with a name. You can call it anytime.

Syntax:

<returnType> <methodName>(<parameters>) {
    // code
    return value; // if needed
}

 Examples:

 void SayHello() {
    Console.WriteLine("Hello!");
}

int Add(int a, int b) {
    return a + b;
}

bool IsEven(int number) {
    return number % 2 == 0;
}

Explanation: 

Methods are like mini-programs inside your program. They make your code reusable, readable, and organized. You can pass values into them and get results out.