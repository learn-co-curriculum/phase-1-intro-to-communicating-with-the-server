# Communicating with the Server

## Learning Goals

- Recall our Three Pillars of Web Programming
- Describe the process of communicating with the server
- Define AJAX

## Introduction

We're two-thirds of the way through our exploration of using JavaScript with the
DOM. We know how to navigate and change the DOM and we know how make and
recognize events. Along the way, we picked up necessary bits of JavaScript. Now
we're getting ready to pull it all together.

## Recall Our Three Pillars of Web Programming

Remember our pillars? By this point, they should feel familiar, but it's
worthwhile to refer back to them as we move along to keep our journey in
perspective. So, in that spirit, our three pillars of web programming are:

- Manipulating the DOM
- Creating events
- Communicating with the server

The last piece, how we send and retrieve information from the server, is what we
need to complete our "favoriting" app.

## Describe the Process of Communicating With the Server

In our Simple Liker app, “favoriting” is a click event on a heart icon that
updates the user’s DOM to show a full heart.

![working example of favoriting a post][three-pillars-example-working]

This event kicks off a sequence of actions to notify the server, so that the
original poster can be notified that you favorited it. JavaScript needs to send
a message to the server when the `click` event runs, and the server needs to
indicate success so that the DOM can update accordingly.

The user doesn't see this entire process happening. Ideally, the process moves
quickly enough that the user barely even notices that it's taken place. All they
know is that the little heart icon is now reflecting their clicked appreciation.
To keep the user experience fast and smooth, we use something called the _AJAX
technique_.

## Define AJAX

_AJAX_ is the shortened version of "asynchronous JavaScript and XML," and it's the
general way we make requests to the server without reloading the web page, and
then work with data we receive from the server. We give the user HTML and CSS
first, then JavaScript, behind the scenes, fills in the rest of the action we
want the page to offer. There are a few different ways to do this technically,
and next we'll take a look at one of the most efficient ways: `fetch()`.

## Conclusion

The last skill we need to be effective JavaScript web programmers is
communication with the server, which links together what we've learned about how
to manipulate the DOM and how to work with events. With the AJAX technique,
we'll learn how to send and recieve data quickly so that we keep our users'
experience a positive one.
