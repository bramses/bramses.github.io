---
layout: post
title: Lexical Scoping in Javascript and Improv
comments: True
---


<figure style="margin-left:25%;">
  <img src="{{site.url}}/assets/pics/improvtim.jpg" alt="The US #1 Improv Team Knife Fighters" width="400" height="auto">
  <figcaption><em>Squad Goals</em></figcaption>
</figure>

## Summary

1. What is lexical scoping?
2. What are closures?
3. Lexical scoping is a technique used in improv
4. Comedic callbacks and Rule of Three

## What is lexical scoping?

Lexical scoping is a computer science concept used to manage and read variables. Lexical scoping is used by the parser (the interpreter of our code) to determine which variables belong to which scope. This is best illustrated with an example:

Some key words:
* variable: a value that can change over time, not constant
* function: a block of code that can be run by a computer by "invoking" it using parentheses, like putOnPants()
* closure: we'll get to that soon ;)

{% highlight javascript %}
function sayMyName() {
  let name = 'Bram'; // name is a local variable
  function displayName() { // displayName() is the inner function, a closure
    console.log(`Hi ${name}!`); // use variable declared in the parent function    
  }
  displayName(); // call displayName
}
sayMyName(); // call sayMyName
{% endhighlight %}
_example courtesy of [Mozilla](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Closures)_

You can run this in your Console too! On Chrome you can hit `⌘-Option-J` `(Ctrl-Shift-J on Windows)` and copy pasta the code above. Feel free to have it say your name instead!

## What are closures?

Closures are similar to lexical scoping, but provide us different benefits. Above, we called `displayName` immediately. However, in Javascript, functions are considered as _first class objects_. All this means is that we can treat functions as objects (an object is a complex topic, but it's easiest to think of as an entity, like a person or a car). Lets modify our example above a bit:

Key Terms:
* return: a return statement is the final line of code in a function. It basically _returns_ the computation done

{% highlight javascript %}
function sayMyNameClosure(name) {
  // we don't need our local variable anymore since we're passing name as an argument
  function displayName() { // displayName() is the inner function, a closure
    console.log(`Hi ${name}!`);  
  }
  return displayName; // return displayName
}
let sayBram = sayMyNameClosure('Bram');
let sayBradPitt = sayMyNameClosure('Brad Pitt');

sayBram(); // call sayBram
sayBradPitt(); // call sayBradPitt
{% endhighlight %}

What's happening here is that we're setting up two separate lexical scopes. These scopes are unique, and both have a different idea of what `name` evaluates to. In `sayBram` name = Bram, but in `sayBradPitt` name = Brad Pitt. Feel free to try these out in your console!

<figure style="margin-left:25%;">
  <img src="{{site.url}}/assets/pics/bradpitt.jpeg" alt="Fight Club" width="400" height="auto">
  <figcaption><em>First rule of closures: don't talk about closures</em></figcaption>
</figure>

## What does this have to do with improv??

I agree, that's enough code, let's focus on comedy here. In improv comedy, the structure usually goes as follows: the audience gives your team a word or a phrase, you spend 20-30 seconds coming up with scenes about it, and then you go wild. The great thing about improv is that it's all based on `Yes, and`, which means that everything your team members say is "true" for the scene. 

Okay, so let's say the word is _typewriter_. I might come up with a scene about how I work at a 1950's news company, Mad Men style. My partner and I would act the scene, and pay attention to which bits get laughs. We then would store those away with the character for later. 

### Example:

__Scene 1__: (Me and one other person) I'm a distraught house husband whose novels aren't taking off because they're really bad. However, my wife doesn't want to shatter my confidence so she tries to stifle her laughter as she reads my book.

__Scene 2__: (Two other people) A completely different timeline where typewriters are falling from the sky, causing mass hysteria. Kind of like Fahrenheit 451 meets dinosaur asteroid extinction.

__Scene 3__: (Me and someone from scene 2) We both narrow in on what went well with the audience the last two scenes and really send those jokes to the moon (as in, we make them even bigger and crazier)

What we're doing here is lexical scoping! We're remembering who our characters were and what they did, and then were invoking them later, like `tellFunnyJokeFromEarlier()`. I won't act as someone else's character and use their jokes, and they won't use mine!

## Rule of Three

I want to close this out discussing the [rule of three](https://en.wikipedia.org/wiki/Rule_of_three_(writing)). The rule of three basically states that jokes are really funny if you use them three times. The rule of three also applies to photography in the Rule of Thirds (another post for another day), and slogans like _Stop, Drop and Roll_. Three is just a really memorable number. So using what we've learned above we can write improv comedy as code like this:

{% highlight javascript %}
function funnyJoke(person) { // pass in our person into the scope
    function tellJoke(joke) { // pass in joke when we call funnyJoke
        console.log(`${person}: ${joke}`);
    }

    return tellJoke;
}

const bramJoke = funnyJoke('Bram');
const bradJoke = funnyJoke('Brad Pitt');

bramJoke('What\'s the deal with airline food?'); // first time
bradJoke('Q: What is Homer Simpson\'s favorite ice cream? \nA: Chocolate-chip cookie d\'oh!')
bramJoke('What\'s the deal with airline food?'); // second time
bradJoke('Q: Why is the math book always upset?\nA: Because it has a lot of problems.')
bramJoke('What\'s the deal with airline food?'); // third time -- audience dies of laughter

{% endhighlight %}