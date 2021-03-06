# Introduction

I remember my first foray into forms. At the turn of the century, web design was one of the modules on the Information Communication and Technology course I took at sixth form college. My learning mostly consisted of cutting and pasting snippets of HTML, CSS, and Javascript. Yes, I came from the view-source school of web design and development.

My obsession with *forms* started when—like with any other HTML element—I tried to cut and paste it. Despite rendering okay, when I submitted it, nothing happened. Fast forward 17 years and here I am writing a book about form design patterns.

## Why Forms?

Every meaningful interaction that happens on the web is achieved by a form of some sort. That's because without forms the web merely becomes a passive experience—just a way to consume content. 

Forms are the vessel by which users can create, update and delete things. Whether it's communicating through email, buying a product, online banking or working on a fully-fledged administrative digital service, forms are always front and center.

Forms, on first glance, are rather easy to grasp. In less than an hour, you'll have text boxes, radio buttons and select boxes on the page. But, their low barrier to entry turns them into what Heydon Pickering refers to as a *10,000-volt electromagnet for attracting usability problems*[^1].

This is a big part of why I'm even writing this book. Typically, these usability problems come up again and again.

## Why Patterns?

Design patterns serve as guidance and solutions to those solving similar problems over and over. The reason for design patterns is twofold.

First, instead of solving the same problem from scratch every time, we can instead use previously designed, available, recognised and well-researched solutions. Ultimately, this saves a lot of time. And really, we can use that time to solve newer and perhaps bigger problems.

Second, by solving the same problem, in the same way, users get a consistent and more coherent experience. The service, app or whatever it is, becomes familiar. Familiar interfaces require less effort to operate. Think about it: every time you encounter a door, you just *know* that it can be opened, closed and sometimes locked.

Leveraging design patterns for digital experiences, or more specifically, forms, makes sense too. By the end of the book, you'll have many patterns that you can use in your own interface immediately.

## Why These Forms?

I first outlined the book based on 50 principles. Originally, each of those would become a short chapter. For example, there was a chapter called “Always Use A Label” and another called “Placeholders are problematic.”

There are a few problems with this approach to design. First, rules can be broken—occasionally. Second, evaluating problems by principle is constraining. Many go together: when talking about screen readers, for example, it often makes sense to discuss keyboard users. And sometimes you have to make trade-offs.

Instead of revolving the book around principles, I decided to revolve it around real problems. That way we can solve them as we do at work. The result is ten specific problems to solve, each represented as a chapter. The chapters are specific, but most of the patterns born out of them are reusable and transferable to many other forms you might be designing. After all, a pattern should be unique, but reusable across projects and organisations.

Here's a chapter run down.

### 1. A Registration Form

We'll start with a basic registration form which makes room to look at the foundational qualities of a well-designed form and how to think about them. By applying something called the Question Protocol, we'll look at how to reduce friction without even touching the interface. Then we'll look at some crucial patterns including validation that we'll want to use for every form.

### 2. Checkout

The One Thing Per Page design pattern is a cornerstone of creating well-designed forms. We'll look at why that is before applying it to a checkout flow. After that, we'll consider flow and order with a view to breaking down each step of the checkout flow. At which point we'll look at several input types and how they affect the user experience on mobile and desktop browsers. All the while, looking at ways to help both first-time and returning customers order quickly and simply.

### 3. Book A flight

We'll dive into the world of progressively enhanced, custom form components using ARIA. We'll do this by exploring the best way to let users select destinations, pick dates, add passengers and choose seats. We'll analyse native form controls at length and look at breaking away from convention where it becomes necessary.

### 4. A Login Form

We'll look at the ubiquitous login form. Despite its simple look, there's a bunch of usability failures that so many sites suffer from. Social media login hasn't necessarily helped matters so we'll look at that too.

### 5. An Inbox

We'll design ways to manage and action email in bulk. This is the first look at administrative interfaces. As such, this comes with its own set of challenges and patterns, including a responsive ARIA-described action menu, multiple selection and same-page messaging.

### 6. A Search Form

We'll look at how to design a responsive search form that is readily available to users on all pages. We'll also look at the importance of the search mechanism that powers it. Together, search can be discoverable, simple and useful.

### 7. A Filter Form

We'll look at how users can filter a large set of unwieldy search results. Without a well-designed filter, users are bound to give up. Filters pose a number of interesting and unique design problems that may force us to challenge ‘best practice’ to give users a better experience.

### 8. An Upload Form

Many services let users upload images and documents. We'll look at the file input and how we can use it to upload multiple files at once. We'll then look at the intricacies of a drag and drop, AJAX-enhanced interface that is inclusive of keyboard and screen reader users.

### 9. An Expense Form

We'll look at the special problem of needing to create and add lots of expenses (or anything else) into a system. Ultimately, this is an excuse to look at the Add Another patern which is often useful in administrative interfaces.

### 10. A Really Long Form

Some forms are really long and take hours to complete. We'll look at some of the patterns we can use to make long forms easier to manage.

## What About Principles?

While I've moved away from principle-orientated chapters, there is still an important place for principles in this book. Without principles, it's hard to know whether what we've designed is objectively good. 

But where should our principles come from? We can either steal other people's, or we can define our own. But before we get to that, let's take a look at how we get to certain principles in the first place.

Our principles normally stem from a belief system. We believe something should be a certain way. We normally have good reason for this. Without a good reason for our belief system, principles crumble under scrutiny.

This book is about designing forms for use on the web. As such, it would be remiss of me to ignore the essence of the web itself. The very power of the web is one of reach and accessibility. Anyone with a browser and an Internet connection gets to use it. And so the principles in this book need to align with this notion—to uphold its inherent qualities.

Frank Chimero talks about this at length in The Web's Grain[^2], one of my favourite articles on design. The main point of which is not to aim to tackle complexity, but to do our very best to avoid it in the first place. Mostly by “going with the grain” and embracing the web's constraints.

It turns out that not only is this the easiest and cheapest way to design something, but that users have a better time operating these simple interfaces in the end too. It's the content and functionality users want anyway.

Whatever we build, in the end, is about users. I don't want to leave a single person behind if I can help it. The web is for everyone. Therefore, I can't think of a better set of principles than the Inclusive Design Principles[^3]. These principles are about good design and good design is inclusive.

1. **Provide a comparable experience**. Ensure your interface provides a comparable experience for all so people can accomplish tasks in a way that suits their needs without undermining the quality of the content.
2. **Consider situation**. People use your interface in different situations. Make sure your interface delivers a valuable experience to people regardless of their circumstances.
3. **Be consistent**. Use familiar conventions and apply them consistently.
4. **Give control**. Ensure people are in control. People should be able to access and interact with content in their preferred way.
5. **Offer choice**. Consider providing different ways for people to complete tasks, especially those that are complex or non standard.
6. **Prioritise content**. Help users focus on core tasks, features, and information by prioritising them within the content and layout.
7. **Add value**. Consider the value of features and how they improve the experience for different users.

We'll refer back to these principles throughout the book, pointing out where a something works or not. These principles should, at least, indirectly hold us to account throughout the design process.

By looking at common form patterns through the lens of inclusivity, this book will help you learn how to apply and reuse conventions that help users complete the task, regardless of how they choose or need to use your service.

## Footnotes

[^1]: https://shop.smashingmagazine.com/products/inclusive-design-patterns
[^2]: https://frankchimero.com/writing/the-webs-grain/
[^3]: http://inclusivedesignprinciples.org/
