

# Clients
_Client_ refers to the part of an app that runs on a device like your computer
or phone. Web apps run in a browser on your device like Chrome, Safari, Firefox,
or Edge.

Clients talk to servers over networks. All browsers (a common _client_) support
three key technologies.

* HTML
* CSS
* Javascript (not to be confused with Java - they're two different things)

You've heard the phrase "form and function".

HTML and CSS **mostly** affect how things _appear_ (i.e. "form") when a user looks
at a screen in your app. Sometimes this is referred to as the _View_ layer of
an app, or what people see.

In contrast, Javascript **mostly** determines how things _function_. How your
app responds when a user does stuff like clicking, typing, scrolling, or
entering data (like their user name and password) in a form.

Every web app uses HTML, CSS, and Javascript so every developer who wants to
write _client_ code that runs in a web browser needs to know them.

Let's compare these three parts to a house.

## 1. HTML = Frame
HTML, or Hyper Text Markup Language, is the frame or underlying _structure_ of
client code that runs in a web browser. It determines the overall shape of
what users see when they look at your app.

When you look at HTML code, you see this hierarchical or nested structure of
_elements_.

![image](https://user-images.githubusercontent.com/1587516/193469943-7eff5924-7fa7-4a4e-83d0-6454aaca510b.png)

[See the code file here](./docs/examples/html-plain.html)

The top level of the structure is an ```<html>``` element. This has _child_
elements like ```<head>``` and ```<body>```, which also have children.

We use tabs in the code to make it easier to see this
hierarchy. The browser knows how to read HTML and convert it into
output on a screen like this:

<img width="408" alt="image" src="https://user-images.githubusercontent.com/1587516/193468907-8dc37523-2728-4868-b1b6-9e4d42cad268.png">


## 2. CSS = Cosmetics
CSS, or Cascading Style Sheets, is the visible layer put over the top of your
house's frame, like paint or siding.

Default styles look very plain. Usually you want your HTML to have
unique colors, fonts and font sizes, spacing, borders, etc. to consistently
reflect your brand.

Here is the HTML above modified with some gaudy styles to make it obvious.

<img width="548" alt="image" src="https://user-images.githubusercontent.com/1587516/193472714-03a46ff4-a0cd-4930-87da-ef7bd6aa059e.png">

[See the code file here](./docs/examples/html-with-css.html)

## 3. Javascript = Wiring and Plumbing
Javascript is about _functionality_. Like the wiring or plumbing that gives a
house electricity and running water, it makes your app function.

When you want your app to _do stuff_, you need Javascript. To continue the
example, we'll add a button. When you click it, the page's title changes from...

<img width="546" alt="image" src="https://user-images.githubusercontent.com/1587516/193473095-2250815f-ba41-41b2-bb1b-019467f5f189.png">

... to

<img width="550" alt="image" src="https://user-images.githubusercontent.com/1587516/193473205-887be2ec-0d1d-4f2b-8134-f859a1889b7d.png">

This was a trivial example to show the concept. When your "client"
needs to talk to a "server" over a network, it's usually doing it with Javascript.
When you want to save data in the browser so you don't have to keep asking the
server for it (way slower), it's using Javascript.

## Front-end Frameworks and Libraries
In the past, the server would generate all the code the browser needed to show
a web page. Every time you clicked a link on a website, you were used to the
short delay required to talk to a server over a network and display the next
web page with a new URL.

Today, SPAs (single page apps) are huge. When you click a link, you don't see
the next page loads. It feels faster.

It's common to do this with _frameworks_ or _libraries_ like React, Angular, Vue,
Typescript, Bootstrap, SASS, LESS, or Tailwind. These are all just ways of
creating, you guessed it...

**HTML, CSS, and Javascript**

Browsers don't know how to interpret Angular or React or LESS. These tools just
make it easier to create good HTML, CSS, and Javascript.
