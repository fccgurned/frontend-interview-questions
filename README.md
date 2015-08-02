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

```
// what logs out here?

var fullname = 'John Doe'
var obj = {
    fullname: 'Colin Ihrig',
    prop: {
        fullname: 'Aurelio De Rosa',
        getFullName: function() {
            return this.fullname;
        }
    }
};

console.log(obj.prop.getFullname());

var test = obj.prop.getFullname;

console.log(test());

// now fix it so the last console.log() prints 'Aurelio De Rosa'
```

```
// the following recursive code will cause a stack overflow if the array is too large.
// how can we fix this and still retain the recursive pattern?

var list = readHugeList();

var nextListItem = function() {
    var item = list.pop();

    if (item) {
        // process the list item...
        nextlistItem();
    }
};
```

```
// what will alert out here?

var a = 'value';

(function() {
    alert(a);
    var a = 'value2';
    })();
```

```
// the following code will output 'my name is rex, Woof!' and then 'my name is, Woof!' one second later.
// fix it so it prints correctly the second time

var Dog = function(name) {
    this.name = name;
}

Dog.prototype.bark = function() {
    console.log('my name is ' + this.name + ', Woof!');
}
var rex = new Dog('rex');

rex.bark();

setTimeout(rex.bark, 1000);
```

```
// the following code is outputting the array, but it's filled with every number
// we just want the even numbers. what's wrong?

var evenNumbers = [];

var findEvenNumbers = function(i) {
    if (i % 2 === 0)
        console.log(i, 'is an even number, adding to array!');
        evenNumbers.push(i);

    for (var i = 0; i < 10; i++) {
        findEvenNumbers(i);
    }
}

console.log(evenNumbers);
//outputs:
//0 "is an even number, adding to array!"
//2 "is an even number, adding to array!"
//4 "is an even number, adding to array!"
//6 "is an even number, adding to array!"
//8 "is an even number, adding to array!"
//[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
```

```
// the following outputs 0, but if 4^2 = 16 and 2^2 = 4,
// then the result should be 12

var square = function(number) {
    result = number * number;
    return result;
}

result = square(4);
result2 = square(2);
difference = result - result2;

console.log(difference);
```

```
+ Write a function that, when passed an array of numbers, gives you the maximum difference between the largest and smallest number ONLY if the smaller number appears before the largest.

For example, [3, 4, 8, 1] = 5. The smallest number is 3, the largest is 8.

This is a refactored (in presentation, not implementation) of the [Stock Price question on Interview Cake](https://www.interviewcake.com/question/stock-price).

+ fizzbuzz

+ I was presented with an HTML element with a border, and asked to animate it left to right for the full width of the browser.

+ I was presented with another HTML box and asked the center it horizontally and vertically
```
