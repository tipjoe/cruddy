# Engineering Mindset
Are you trying to be a Programmer, Developer, or an Engineer?

A **programmer** knows how to _use a specific tool for a specific thing_.
Like a cook at a
fast food restaurant that drops pre-cut frozen fries into a fry basket and
take them out when a bell dings. It doesn't take a lot of training.

A **developer** understands a _variety of tools and when to use them_. Like a
cook who can take a variety of orders and how to make them.

An **engineer** knows how to _make the tools they need_. Like a chef who can
invent new dishes by understand ingredients and how they interact.

In practice, these names often get used interchangably. It's important to
understand the different levels of insight needed for each.

The goal of an engineer isn't to become a PHP, Java, or React developer. When
you're looking at job listings and wanting to increase your income opportunities
it can be easy to start thinking this way.

Practically speaking, we become skilled with languages or frameworks that allow
us to be productive. But the goal isn't to learn a language or framework. It's
to understand the underlying concepts.

When you understand the building blocks of software (and the hardware it runs
on), you can learn any language or framework more quickly because you know
what you're looking for. Like knowing how to fish. If you know what to look for
you can catch fish in any river. Nobody says, "I'm a Provo River fly fisherman."
They're just a fly fisherman. But we do this with technology when we say things
like, "I'm a React Developer" or "I'm a .NET developer".

Maybe you're more productive in React because you've been using it for months.
But if you know the concepts that drive it, you can switch to Angular or Vue
pretty quickly.

## Syntax and Sementics
Already, these words are sounding hoytie-toytie, so let's look at what they mean.

Kids born anywhere learn how to speak some words.

```I hungry!```

The way they say it (syntax) may be wrong, but their meaning (semantics) is
clear. As they grow up, they'll gradually start saying:

```I'm hungry!```

It still includes a ```subject > verb > adjective``` and has the same meaning
but the syntax is slightly different. What about if you just change one
word?

```I'm stinky!```

The syntax is the same: ```subject > verb > adjective```, but stinky and
hungry have very different meanings (semantics).

What about learning this in Spanish?

```¡Tengo hambre!``` (Spanish for "I'm hungry!")

Here, the syntax is a little different (different words and structure), but the
_semantic_ (meaning) is the same as in English.

This happens a lot in code.

When you think of yourself as a React developer (English), it sounds
intimidating to switch to being an Angular developer (Spanish).

When you think like an engineer rather than a programmer, changing
languages isn't a big deal. You may be a little less productive for a while
while you learn some new syntax, but the semantics, or meaning of what you're
trying to accomplish, will be similar.

You think in terms of the structure of code rather typing the right words
on every line of code.

## A Secret: It's All Functions

Remember functions from junior high math. Something like:

```y = f(x)```

Give a function (f) an input (x) and it returns an output (y). Here's one.

12 = add(3, 4, 5)

The add function's job is to add up the inputs 3, 4, and 5 and return 12.

Software engineers recognize that **all code**, whether front-end, back-end, or
wherever, is just functions.

```Output = a Function that does something to Inputs```

This is true for every software language, framework, or tool. It was true
for computers in the 1950s and it's true for latest ShinyNewThing.

Don't believe me? Let's look at examples across some coding languages.

### HTML
Here's an example with a div. Normally you don't think of an HTML ```<div>```
element as a function, but it is!

```<div class='pl-4' style='border: 1px solid'>I like dogs.</div>```

Function:
* div

Inputs:
* class attribute with a value of 'pl-4'
* style attribute with a value of 'border...'
* inner text with a value of 'I like dogs.'

Outputs:
HTML on a screen with styles and text.

### CSS
Here's a css style function that makes text color red.

```style='color: red;'```

Function:
* style

Inputs:
* style attribute with a value of 'color: red;'
* color property with a value of red

Output:
Red text on whatever HTML element you've attached this function to.

### Javascript
Here's a more traditional looking function named getNamePlusPoop.

function getNamePlusPoop(name) {
    return name + ' Poop';
}

Function:
* getNamePlusPoop

Input:
* name (we'll say it's Joe)

Output:
* Joe Poop

OK, what about other Javascript stuff that isn't a named function?

```Math.add(2, 2, 7)```

Inputs:
* 2, 2, 7 (numbers to add)

Output:
* 11

```const doggy```

Input:
* doggy

Output:
* A a variable named doggy that points to a place in memory where you can save its value.

```document.getElementById('dogcat1')```

Function:
* document.getElementById

Input:
* An ID called dogcat1

Output:
* The HTML DOM element with the ID of dogcat1

Whether it's called a command or a function, it's still a function.

### SQL
What the?! Is SQL a programming language? Yep. It just has the specialized
purpose of talking to a relational database.

Remember how commands are just functions? So are statements, like this
```select``` statement. The _syntax_ (form) is different but the
_semantics_ (meaning) are the same.

```select id, address from users where name = 'J.J. Garglecarp';```

Function:
* select

Inputs:
* id, address - the columns to retrieve
* from users - the table name to get the columns from
* where name = 'J.J. Garglecarp' - filter only results where users.name matches

Output:
* database records that match the inputs

## Shell scripts
Executable shell scripts you run in your terminal are also just functions.

```pwd```

If you type this in your bash or zsh terminal, it tells you the 'present
working directory'. Say I'm at ~/joe/dogfolder but I forgot where I was.

Function:
* pwd

Inputs:
NONE - not all functions have inputs. When a function doesn't require inputs,
it just means that it has a default thing it will do. In this case, it assumes
it's acting on whatever director you're currently in.

Output
* ~/joe/dogfolder

Same goes for ```ls``` or other terminal commands.

<br>
___
<br>

Not convinced? Pick a technology and try it. It might have syntax that looks
very different from these examples, but it's doing the same thing you learned
in junior high.

```y = f(x)```

Give a function (f) input(s) (x) and it returns an output (y).

Sometimes the function does stuff without returning anything. Having a
response (or output) of ```void``` is common.

Regardless of a million different _syntaxes_, they're just different ways to
implement recurring _semantic_ patterns.

Engineers have to learn syntax (form) to use a language, but are more focused
on the semantics (meaning) that cross languages and technologies.

## Encapsulization and Black Boxes
Often, technologies _encapsulate_ functionality in black boxes. Your car does
this. You just need to know how to use the car's interface (steering wheel, gas,
brakes, turn signal, etc.) You don't need to be a mechanical engineer to drive
a car.

This happens on many levels. You don't need to be a network engineer with deep
understanding of TCP/IP, packets, etc... to use networking in your software.

In Javascript, this is all encapsulated in a ```fetch``` command (or function).
You just give it the right inputs and expect the right outputs. This is
sometimes called a black box because you can't see inside of it.

Nobody can learn everything. Instead, we learn the interfaces to various black
boxes with encapsulated functionality we can drive like our cars.

Widely-used protocols like HTTP and DNS are largely black boxes to most, even
engineers. Unless they're the ones who build them. APIs are also black boxes
that expose only the _interface_ you need to use them.