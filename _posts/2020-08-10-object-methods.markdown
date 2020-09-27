---
layout: post
title:  "Object methods"
date:   2020-09-03 19:31:08 +0100
categories: JavaScript
---
In JavaScript, objects are used to store `key`: `value` pairs. There are two types of keys that we can encounter in objects. The first type is `property` used to store simple data like strings or numbers. The second one is `method` which is basicaly a function, but because it's scope is inside an object it is called a method instead.

Let's have a look at a simple object below:

{% highlight JavaScript %}
let obj = {
  name: 'Razvan',
  age: 25,
  isWorking: () => {
    return `Is ${obj.name} working ?`
  }
};

this is a property: obj.name outcome will be 'Razvan'
this is a property: obj.age outcome will be 25
this is a method: obj.isWorking() outcome will be 'Is Razvan working?' 
{% endhighlight %}

If we would try and call the `isWorking` function on it's own, we would get an error saying that the function is not defined. That is true because the function can only be found inside the `obj` object, which is what makes it a method.
This is the difference between methods and functions.

You can read more about the topic below:

[javascript-info]: https://javascript.info/object-methods

