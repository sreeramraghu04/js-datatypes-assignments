# JavaScript

## assignment

1. Who is the founder of JavaScript and when was it
   founded?

   - JavaScript was created by **Brendan Eich** in **1995** while he was working at **Netscape Communications Corporation**. It was initially developed in just **10 days** and was originally called **Mocha**, later renamed **LiveScript**, and finally **JavaScript** when it was released in Netscape Navigator 2.0.

2. What was the first browser, and when was it released?

   - The first web browser was **WorldWideWeb**, later renamed **Nexus**, and it was created by **Tim Berners-Lee** in **1990** while he was working at CERN. It was the first browser capable of displaying web pages and editing them.

3. Name the two dominant browsers in 2000

   - The two dominant web browsers in **2000** were:

   **Internet Explorer (IE)** – Developed by Microsoft, it had the largest market share at the time, especially with the release of **Internet Explorer 5 and 6**.  
   **Netscape Navigator** – Once the leading browser in the 1990s, it was declining in popularity due to competition from Internet Explorer.

   By the early 2000s, Internet Explorer had a significant lead, leading to the eventual decline of Netscape and the rise of Mozilla Firefox later in the decade.

4. What is ECMAScript?

   - **ECMAScript (ES)** is a **standardized scripting language** specification that serves as the foundation for **JavaScript** and other scripting languages like **JScript** and **ActionScript**. It was created by **Ecma International** to ensure consistency and interoperability across different implementations of JavaScript.

   The first edition of ECMAScript was released in **1997**, and it has since undergone multiple updates, with major versions like **ES6 (ECMAScript 2015)** introducing modern features such as **let/const, arrow functions, classes, and promises**.

5. Define syntax.

   - **Syntax** refers to the set of rules that define the structure of a programming language. It specifies how code should be written and formatted so that a compiler or interpreter can understand and execute it correctly. Syntax includes elements like keywords, operators, punctuation, and the proper arrangement of statements and expressions.

   For example, in **JavaScript**, a simple syntax rule is:

   ```js
   let x = 10; // Correct syntax
   let y 10  // Incorrect syntax (missing '=' sign)
   ```

   Incorrect syntax leads to errors and prevents the program from running properly.

6. What is TC39?

   - **TC39** (Technical Committee 39) is the committee responsible for developing and maintaining the **ECMAScript** language, which is the standard upon which **JavaScript** is based. TC39 operates under **ECMA International** and consists of representatives from major tech companies like Google, Microsoft, Apple, and Mozilla.

   ### Key Responsibilities of TC39:

   **Proposing New Features** – Developers and committee members propose enhancements to JavaScript.
   **Reviewing and Refining Proposals** – Features go through a **5-stage process** before being added to the ECMAScript standard.
   **Publishing ECMAScript Versions** – They release new versions of ECMAScript (e.g., ES6, ES7, etc.).
   **Maintaining Compatibility** – Ensuring backward compatibility and improving performance.

7. Name different data types in JavaScript

   - JavaScript has **eight** fundamental data types, categorized into **primitive** and **non-primitive (reference)** types.

   ### **1. Primitive Data Types** (Stored directly in memory)

   **String** – Represents text values.sequence of character enclosed in single or double quotes.

   ```js
   let name = "John";
   ```

   **Number** – Represents both integers and floating-point numbers.

   ```js
   let age = 25;
   ```

   **Boolean** – Represents `true` or `false` values.

   ```js
   let isStudent = true;
   ```

   **Undefined** – A variable that has been declared but not assigned a value.

   ```js
   let x; // undefined
   ```

   **Null** – Represents an intentional absence of value.

   ```js
   let y = null;
   ```

   **BigInt** – Used for handling very large integers.

   ```js
   let bigNumber = 123456789012345678901234567890n;
   ```

   **Symbol** – Represents unique and immutable values, often used as object property keys.

   ```js
   let sym = Symbol("unique");
   ```

   ### **2. Non-Primitive (Reference) Data Type**

   **Object** – a collection of related data enclosed with curly braces separated with comas the properties are written in key value pairs.

   ```js
   let person = { name: "John", age: 25 };
   ```

   **Array** - a collection of datatypes enclosed with square braces separated using comas.

   ```js
   let fruits = ["Apple", "Banana", "Mango"];
   ```

   **Function** - A block of reusable code.

   ```js
   function greet() {
     return "Hello!";
   }
   ```

   **Date** - Represents date and time.

   ```js
   let today = new Date();
   ```

8. Explain primitive and non-primitive data types

   - ### **Primitive vs. Non-Primitive Data Types in JavaScript**

   JavaScript data types are categorized into **primitive** and **non-primitive (reference)** types.

   ***

   ## **1. Primitive Data Types**

   Primitive data types store single values **directly** in memory and are **immutable** (cannot be modified).

   ### **Characteristics of Primitive Data Types:**

   ✅ Stored **directly** in memory.  
   ✅ Immutable (Cannot be changed).  
   ✅ Compared by **value**.

   ***

   ## **2. Non-Primitive (Reference) Data Types**

   Non-primitive data types store **references** (memory addresses) instead of actual values.

   ### **Characteristics of Non-Primitive Data Types:**

   ✅ Stored as **references** in memory.  
   ✅ Mutable (Can be changed).  
   ✅ Compared by **reference**, not value.

   ***

   ### **Key Differences Between Primitive & Non-Primitive Data Types**

   | Feature        | Primitive Data Types                                                   | Non-Primitive Data Types              |
   | -------------- | ---------------------------------------------------------------------- | ------------------------------------- |
   | **Storage**    | Stored directly in memory                                              | Stored as references                  |
   | **Mutability** | Immutable (Cannot be modified)                                         | Mutable (Can be modified)             |
   | **Comparison** | Compared by value                                                      | Compared by reference                 |
   | **Examples**   | `String`, `Number`, `Boolean`, `Undefined`, `Null`, `BigInt`, `Symbol` | `Object`, `Array`, `Function`, `Date` |

9. Differentiate null and undefined

   - ### **Difference Between `null` and `undefined` in JavaScript**

   Both `null` and `undefined` represent **absence of a value**, but they have different meanings and uses.

   ### **Example Code:**

   ```js
   let a;
   console.log(a); // undefined (variable declared but not assigned)

   let b = null;
   console.log(b); // null (explicitly set to "nothing")
   ```

10. What is the difference between undefined and not defined

    - ### **Difference Between `undefined` and "not defined" in JavaScript**

    | Feature          | `undefined`                                         | **"Not Defined" (ReferenceError)**                    |
    | ---------------- | --------------------------------------------------- | ----------------------------------------------------- |
    | **Meaning**      | The variable is declared but has no assigned value. | The variable has never been declared in the program.  |
    | **Type**         | `undefined`                                         | Throws a `ReferenceError`.                            |
    | **Occurs When?** | A variable is declared but not assigned any value.  | A variable is used without being declared.            |
    | **Example**      | `let x; console.log(x); // undefined`               | `console.log(y); // ReferenceError: y is not defined` |

    ### **Example Code:**

    ```js
    let a;
    console.log(a); // undefined (declared but no value assigned)

    console.log(b); // ReferenceError: b is not defined (never declared)
    ```

11. What is the difference WorldWideWeb and World Wide Web

    - ### **Difference Between "WorldWideWeb" and "World Wide Web"**

    | Term                     | Meaning                                                                                                                              |
    | ------------------------ | ------------------------------------------------------------------------------------------------------------------------------------ |
    | **WorldWideWeb**         | The first web browser and editor, created by **Tim Berners-Lee** in 1990. It was later renamed **Nexus** to avoid confusion.         |
    | **World Wide Web (WWW)** | A global system of interconnected web pages and resources accessed via the internet. It was invented by **Tim Berners-Lee** in 1989. |

    ### **Key Differences**:

    - **WorldWideWeb** (or Nexus) was a **software application** used to browse web pages.
    - **World Wide Web** (WWW) is the **network of websites and webpages** accessible via the internet.

12. What is the symbol datatype in JavaScript

    - ### **Symbol Data Type in JavaScript**

    The **`Symbol`** data type in JavaScript is a **primitive** type introduced in **ES6 (ECMAScript 2015)**. It is used to create **unique and immutable identifiers**.

    ### **Key Characteristics of `Symbol`:**

    ✅ **Always Unique** – Even if two symbols have the same description, they are different.  
    ✅ **Immutable** – Once created, its value cannot be changed.  
    ✅ **Used as Object Keys** – Prevents accidental property name conflicts.  
    ✅ **Not Auto-Convertible to Strings** – Unlike other primitives, `Symbol` cannot be automatically converted to a string.

13. What is the difference between is single quote, double quote, and backticks

    - In JavaScript, we can define strings using **single quotes (`'`)**, **double quotes (`"`)**, or **backticks (`` ` ``)**.

    - **Single (`'`) and Double (`"`) Quotes**: Both work similarly for simple strings, but we need to escape quotes if the same type is inside the string.  
      Example: `'It\'s a nice day'` or `"He said, \"Hello!\""`
    - **Backticks (Template Literals) (` ` ` `)**: Allow **multi-line strings** and **string interpolation** using **`${}`**.  
      Example: `` `Hello, ${name}!` ``

# Javascript Simple Quiz on Data Types

- ![alt text](javascript-mcq-on-data-types.html.jpeg)
