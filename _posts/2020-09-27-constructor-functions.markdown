---
layout: post
title:  "Constructor Functions"
date:   2020-09-27 19:31:08 +0100
categories: JavaScript
---

The first letter of the constructor functions name is always an upper case. This is how we can easily differentiate between a normal function and a constructor function. 

I would define constructor functions as a mini factory. You set it up once and then you can have as many instances of that as you'd like. You will need the `new` keyword to do that. This keyword is specific to constructor functions. Let's have a look at an example below to have a clearer picture of how they actually work: 

{% highlight JavaScript %}
class User{
    constructor(name, age) {
    this.name = name;
    this.age = age;
}
    sayHi() {
    return 'Hi' + ' ' + this.name ;
}
}

// class User or our mini factory has been created

// now we are gonna create a new instance and use it

let John = new User('John', 26)  // here we are using the new keyword and pass in the parameters for name and age

// we will now see if it works as expected

John // User {name: "John", age: 26}
John.name = 'John';
John.age = 26;
John.sayHi() = 'Hi John';
{% endhighlight %}