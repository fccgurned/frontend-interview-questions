#Frontend Developer Interview Questions

This repo collects the interview questions from [this Reddit thread](https://www.reddit.com/r/webdev/comments/3f7q3q/been_interviewing_with_a_lot_of_tech_startups_as/)

##Standard Javascript Questions

+ Explain Closures in Javascript
+ Explain Event Bubbling
+ Explain Event Delegation
+ What does `apply()` do?
+ What does `bind()` do?
+ Explain what the `Array.prototype.map()` function does, and provide an example.
+ What is `Strict Mode`?
+ What is the difference between a Promise and a Callback?

##Standard Angular Questions
+ What is Scope?
+ What is a Directive?
+ What is the link function in the Directive?
+ What is the digest cycle?
+ What is `$scope.$apply`?
+ What are the most commonly used, out of the box Directives?
+ What does `transclude` do on directives?
+ Tell me about a time you had problems with state in Angular
+ Have you ever had performance issues in Angular? How did you tackle them?
+ What do you like about Angular?
+ What do you dislike about Angular?
+ Why use the `q` promise library as opposed to just returning a promise from `$http`?
+ What does `$resource` do?

##General/Presentation Layer Questions
+ What is a Model in MVC?
+ Explain CSS Specificity
+ How do you center something horizontally?
+ Explain what media queries are
+ What are the pros and cons of a Single-Page Application?
+ How could you improve the performance of a Single-Page Application?
+ What's the difference between `inline-block` and `inline`?
+ How would you develop a mobile site for a webiste that didn't already have one?
+ What is JSONP?
+ What is a Doctype?
+ On a UNIX command line, how would you run a long command you typed out already an hour ago?
+ What front-end tools do you normally use?
+ Where do you think UI's are headed?
+ What motivates you?
+ How do you learn?

##JS Challenge Questions
Three questions from [You Can't Javascript Under Pressure](http://games.usvsth3m.com/javascript-under-pressure/)

```
function doubleInteger(i) {
    // i will be an integer. Double it and return i.
    return i'
}
```

```
function isNumberEven(i) {
    // i will be an integer. Return true if it's even, and false if it's not.
}
```

```
function getFileExtension(i) {
    // i will be a string, but it may not have a file extension.
    // return the file extension (with no period) if it has one, otherwise false.
}
```

```
// what gets printed to the console here, and why?
(function() {
    var a = b = 5
    })();
console.log(b);
```

```
// create a function, `repeatify`, on the String prototype chain.
// this function accepts an integer that specifies how many times the string has to be repeated.
// the function returns the string repeated the number of times specified, without spaces.

console.log('hello'.repeatify(3)); // 'hellohellohello'
```

