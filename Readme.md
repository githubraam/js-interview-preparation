# Questions
###### Difference between Lexical scope, Scope chain, and variable scope.
###### What is Shadow DOM ? Give some example
###### what you mean by Virtual DOM?
###### Define HOC, Why we should use HOC.
## What is Pure Function?

A Pure Function is a function (a block of code) that always returns the same result if the same arguments are passed. It does not depend on any state or data change during a program’s execution. Rather, it only depends on its input arguments.

Also a pure function does not produce any observable side effects such as network requests or data mutation etc.

**Let’s see the below JavaScript Function:**
```
function calculateGST( productPrice ) {
    return productPrice * 0.05;
}
```
The above function will always return the same result, if we pass the same productPrice. In other words, its output doesn’t get affected by any other values / state changes. So we can call “calculateGST” function a Pure Function.

**Now, let’s see one more function below:**

```
var tax = 20;
function calculateGST( productPrice ) {
    return productPrice * (tax / 100) + productPrice;
}
```
Pause a second and can you guess whether the above function is Pure or not ?

If you guessed that it is isn’t, you are right! It is not a pure function as the output is dependent on an external variable “tax”. So if the tax value is updated somehow, then we will get a different output though we pass the same productPrice as a parameter to the function.

But here we need to make an important note:

Note: If a pure function calls a pure function, this isn’t a side effect and the calling function is still considered pure. (Example: using Math.max() inside a function)

Below are some side effects (but not limited to) which a function should not produce in order to be considered as a pure function –

* Making a HTTP request
* Mutating data
* Printing to a screen or console
* DOM Query/Manipulation
* Math.random()
* Getting the current time

## Define High order Function? why function are called first class citizen?

If any programming language has the ability to treat functions as values, to pass them as arguments and to return a function from another function then it is said that  programming language has First Class Functions and the functions are called as First Class Citizens in that programming language.

Functions are very important and powerful in JavaScript. JavaScript has all those abilities or features that are required to be a language having First Class Functions, hence functions are treated as First Class Citizens. Let’s look at all the abilities of functions being a First Class Citizen.

**Ability to treat functions as values**
``` 
<script>
  var greet = function() {
    console.log("Welcome to GeeksforGeeks!");
  }
  greet();
</script> 
```

**Ability to pass a function as arguments**
```
<script>
function teacher(){
    return "Teacher";
}
  
function student(){
    return "Student";
}
  
function greet(user){
    console.log("Welcome", user());    
}
  
// Prints "Welcome Teacher"
var message = greet(teacher);
  
// Prints "Welcome Student" 
var message = greet(student);
</script>
```

**Ability to return a function from another function**
```
<script>
var greet = function(){
    return function(){
    console.log("Welcome to GeeksforGeeks!");
    }
}
greet()();
</script>
```

###### Why REACT contributer suggest to use functional component instead of class component?
###### How to prevent rerender of component in REACT? Difference bw useCallback and useMemo hooks?
###### What is Temporal Dead Zone in JS?
###### Difference bw var, let and const with example?
###### What you mean by closure and hoisting?
###### difference bw ASYNC, await and Promise?
###### REACT: Suspence, Lazy Load, Error boundaries?
###### Difference bw DOM and BOM in js?
###### Event Loop?
###### Event Bubbling and Capturing?
###### Call, apply,bind and polyfills for each?
###### Difference between useState and useReducer?
###### Difference between state and props?
###### How to perform lifecycle methods in functional component?
###### Event garbage collection?
###### useEffect cleanup example?
###### what is function currying?
###### Event Loop online platform link [Online Eventloop platform](https://www.jsv9000.app/).


## HTML AND CSS QUESTIONS
###### Why we need Doctype declaration in html page? What happen if we not use doctype?
###### How to make full screen equal column in bootstrap

## Nagarro
###### what is code splitting in reactjs?
###### what is difference bw code spliting and lazy load?
###### when do we prefere lazy load of our components?
###### why do we use REACT-ROUTER?
###### what are the latest chanages introduced in REACT-ROUTER?
###### what is error boundary and can we implement it in reactjs?
###### can we implement error boundary in functional component?
###### Difference bw redux thunk and saga?
###### why do we use Generator function?
###### what will happen if call generator function without next()?
###### how to delete all localstorage in one go?
###### define diff techniques to create object?
###### reason behind preferening Object.create method for creating Objects?

### css
###### new things in bootstrap 5?
###### how can we add Sass in react project?
###### why ::after and ::before call as psedo elements?
