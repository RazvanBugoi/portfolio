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
{% endhighlight %}

Where `YEAR` is a four-digit number, `MONTH` and `DAY` are both two-digit numbers, and `MARKUP` is the file extension representing the format used in the file. After that, include the necessary front matter. Take a look at the source for this post to get an idea about how it works.

Jekyll also offers powerful support for code snippets:

{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
