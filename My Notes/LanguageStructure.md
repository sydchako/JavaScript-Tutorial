## JavaScript code structure

To be a good developer, you need to know the building blocks of the language you will be using. We are going to look at statements first.

## Statements

A statement is a command that performs an action. There virtually is no limit to the number of statements any piece of code can have. The example below shows what some JavaScript statements look like:

```Js
let a = 2;
let b = 3;
let c = a + b;
``` 

The example above is a piece of code that has only 3 statements. The first statement assigns a value of 2 to the variable ``a``. The second statement assigns a value of 3 to the variable ``b``. The final statement takes the sum of ``a`` and ``b`` and assign it to variable ``c`` which means the value in variable ``c`` is now 5.

For code readability, each statement is written on a separate line.

The same code above can be written as:

```Js
let a = 2; let b = 3; let c= a + b;
```

As you can see now, the code becomes less readable.

Its very important to write readable code because:
* it makes the process of finding bugs (unintentional code behavioral errors) easier. That process is called debugging.
* it makes it easier for your team to understand your code if you are working as a team.
* it makes it easier for you to maintain and upgrade your code later when you decide to add new ideas.


## Semicolons

```Js
let a = 2;
let b = 3;
let c = a + b;
``` 

Looking at the code above you might have noticed that each of my statements is ending with a semicolon (;). A semicolon is a way of explicitly notifying the JavaScript engine about the end of a statement.

However, JavaScript in **most** cases interprets a line break as an implicit semicolon which therefore means semicolons are optional in JavaScript. What this means is that the code below is also valid even though it lacks semicolons:

```Js
let a = 2
let b = 3
let c = a + b
```

In some programming languages such as C, C++ and Java, the semicolon is compulsory and missing it means the code wont even compile. In Python, the semicolon is not needed at all. Here in JavaScript, its usually optional.

Even though the semicolon is optional in JavaScript, it is good practice to end all JavaScript statements with semicolons. The reason is that there are some cases where missing a semicolon produces unintentional results even though the code runs.

In short, never leave the semicolon.

## Comments

JavaScript has two types of comments:
* single-line comments which start with two forward slash characters `//`
* multi-line comments which start with a forward slash and an asterisk <code>/&#42;</code> and end with an asterisk and a forward slash <code>&#42;/</code>

```js
// This is a single-line comment
// This is another single-line comment
```

```Js
/* This is a multi-line comment
which is used when the comment
spans many lines */
```

Comments are ignored by the JavaScript engine which means they don't affect the execution of the code. The program works the same whether the comments are there or not.

As your code grows you end up possibly having hundreds or thousands of statements, some of them very complex. When dealing with such bigger programs you eventually reach a point where you revisit a certain part of your code and become clueless about the purpose of that part you wrote sometime ago. It therefore becomes important to label parts of your codes with comments to help you later when debugging or maintaining your code.

Here is an example showing basically how you can label a piece of code using single line comments.

```Js
// codeblock to find the sum of two variables
let a = 2 
let b = 3
let c = a + b
//-- end of the block
```

Comments are also useful again when debugging a program. Lets say you have a program producing unexpected results and there are certain statements you suspect are causing it. You first comment out the statement and test the code to see how it behaves without that statement. This is better than deleting the statement because later you might find that it was the one misbehaving. In that you would simply have to remove the commenting on the statement.

Here is how you comment out a statement:

```Js
let a = 2 
let b = 3
// let c = a + b
```

Here is how you comment out a block:

```Js
/* 
let a = 2 
let b = 3
let c = a + b 
*/
```

Or better still, you can include the reason why the block was commented out.

```Js
/*** This part was causing a bootloop ***
let a = 2 
let b = 3
let c = a + b 
*/
```

Earlier on I mentioned that comments don't affect the execution of the code, however they increase the size of the code (code footprint) which increases the load time of the code. That is undesirable but still not a problem at all. There are many tools specifically designed to minify the code before publishing. The comments will be removed, so they don't appear in the working scripts. So don't be afraid of commenting your code.
