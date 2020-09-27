---
layout: post
title:  "For in loop"
date:   2020-09-27 19:31:08 +0100
categories: JavaScript
---

The for in loop is a special type of loop used to parse through keys and/or values in objects. It can also be used to parse through arrays. Let's have a look over how it works.

{% highlight JavaScript %}
let obj = {
 name: 'Razvan',
 age: 25,
 employment: 'full time',
 gender: 'male',
}

for (ley keys in obj) {
    console.log(keys) // this will output each key
    // name
    // age
    // emplyoment
    // gender
}

for (let keys in obj) {
    console.log(obj[keys]) // this will output each value
    // 'Razvan'
    // 25,
    // 'full time'
    // 'male'
}


// it works for arrays too:

let arr = [1,2,3,4,5];

for (let value in arr) {
    console.log(arr[value]) // will output all the elements of the array
    // 1
    // 2
    // 3
    // 4
    // 5
}
{% endhighlight %}