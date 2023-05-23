# Introduction to Communicating with the Server

## Learning Goals

- Recall our Three Pillars of Web Programming
- Define clients and servers
- Define AJAX

## Introduction

We're two-thirds of the way through our exploration of using JavaScript with the
DOM!

We know how to navigate and change the DOM and we know how to make and recognize
events. Along the way, we picked up necessary bits of JavaScript.

Now, we're getting ready to pull it all together!

## Recall Our Three Pillars of Web Programming

Remember our three pillars of web programming? They are:

- Manipulating the DOM
- Creating events
- Communicating with the server

This last piece - sending and requesting information from the server - is what
we need to complete our "favoriting" app.

## Communicating With the Server

In our Simple Liker app, “favoriting” is a click event on a heart icon that
updates the user’s DOM to show a full heart.

![working example of favoriting a post][three-pillars-example-working]

At this point, we're capable of handling a click event and changing what the
user sees on our webpage. But, if we refresh the page, that information goes
away! Our liker app isn't working the way we want it to just yet.

When a user "likes" a post, they're giving us a piece of data - "I, user X, like
this post!"

We want that data to _persist_ in our application. When something
_persists_, it lasts between page refreshes. In order for our data to persist,
we need a place to store it.

This is where the process of communicating with the server comes in!

### Clients

So far, we've been working entirely in the client, writing client-side code. In
development, a _client_ is the visual interface that users engage with to
interact with an app. As web developers, our client is the browser, but _client_
can refer to other types of user interfaces as well, like mobile apps.

Clients are responsible for displaying a user interface and handling user
interaction. That's the job of HTML, CSS, and JavaScript - to structure and
style a webpage and make it interactive and dynamic.

### Servers

Servers have a different job - they're remote, independent computers that are
responsible for storing the files of our website, communicating with databases,
and running the code that makes our website accessible over the internet.

Servers do a lot! You can think of them as a _home base_ for our websites -
they're where our websites actually live!

In order for us to build fully functional web apps, our client-side code needs
to be able to communicate with a server.

We'll need to be able to ask our server for data, send data to our server so
that the server can persist that data in a database, update data that we're
already storing, and remove data that we no longer want to store.

Imagine, for example, that you're designing YouTube. You'll need to be able to
serve people videos based on a search - requesting data - allow people to post
new videos - persisting data - update the number of likes associated with a
video - updating data - and allow people to remove videos that they no longer
want to keep - deleting data.

Whew! That's a lot to do!

Fortunately, JavaScript makes it easy for us using the _AJAX_ technique.

## Define AJAX

_AJAX_ is short for "asynchronous JavaScript and XML". It's the process used to
make requests to the server and update the DOM without reloading the web page.

There are a few different ways to implement this. We'll take a look at one of
the most efficient ways: `fetch()`.

The name "asynchronous JavaScript and XML" arises from the fact that, in the
past, the data sent back to the browser from the server was encoded as XML.

Now, however, it's most often sent back in a format known as JSON ("Jay-Sawn").
JavaScript Object Notation (JSON) is a `String` that JavaScript knows how to
turn into an `Object`. Using JavaScript, we can access the JSON returned by the
server and use it to update the DOM.

## Conclusion

The last skill we need to be effective JavaScript web programmers is
communication with the server. Once we've mastered this final step, we will be
able to listen for an event, persist the change to the backend, and manipulate
the DOM to reflect the updated information.

In coming lessons, we'll learn more about how the web works and how to use the
AJAX technique. We'll cover concepts like `fetch`, `JSON`, and `asynchronous
javascript` in greater detail, so don't worry if you don't feel familiar with
those concepts at this point! By the end of this module, you'll be able to
identify and describe each of those terms and implement them in your code.

[three-pillars-example-working]:
    https://curriculum-content.s3.amazonaws.com/fewpjs/fewpjs-stitching-together-the-three-pillars/three-pillars-02.gif
