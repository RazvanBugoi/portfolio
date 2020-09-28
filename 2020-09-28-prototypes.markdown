---
layout: post
title:  "Prototypes"
date:   2020-09-28 19:31:08 +0100
categories: JavaScript
---

In JavaScript, objects have a special hidden property called `[[Prototype]]` that is either `null` or references another object. That object is called a prototype.

If we want to read a property from an object and it's missing, JavaScript automatically takes it from the prototype if it's there. This is called prototypal inheritance.

Let's see an example below to understand how this works: 

{% highlight JavaScript %}
let fruits = {
    vitaminC: true,
};
let orange = {
    isSweet: true,
}

orange.__proto__ = fruits; (**)
//now we can find both properties in orange object
orange.isSweet //  true;
orange.vitaminC // true;
{% endhighlight %}

at ** we tell the engine that orange now has `fruits` object as it's prototype. Then, when we call the vitaminC property on orange object, the engine will search for it in it's prototype which we have set to be `fruits` object. This is how prototypal inheritance works. 
