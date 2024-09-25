---
layout: essay
type: essay
title: "Coding with Constraints: Navigating ESLint's Challenges"
# All dates must be YYYY-MM-DD format!
date: 2024-09-25
published: true
labels:
  - ICS 314
  - Coding Standards
  - ESLint
---
Going from implementing coding standards from my earlier courses on Java to trying to fix every single ESLint error proved to be incredibly difficult. Basic coding problems take twice as long when you’re adhering to ESLint's rules, and the solution that you might have used to solve the problem might not even work! ESLint was especially hard to work with when using array functions since ESLint is so particular with the syntax you use. For example, when doing the assignment E27, I ended up having to change a plethora of things that would normally work fine. This included changing my array from type: any[] to using type generics to remove an ESLint error that wanted a specific datatype, not using a return statement with the reduce function to remove an “Unexpected block statement” error because it was deemed unnecessary, and even making sure to put a space before and after mathematic symbols. Did ESLint help my code look nicer? Yes, but I do not think it was worth all the headache.

## Using ESLint in the future?

Despite my frustrations, I still do think ESLint is a great tool to help developers ensure their projects are uniform no matter how many collaborators are involved. In Typescript, developers have some flexibility in the amount of quotes you want to use for a string or how to concatenate a string properly, and ESLint ensures that everyone will implement their coding solutions the same way. I encountered this myself when I tried to return a string to the console and received an ESLint error for not properly concatenating my string. Instead of having: “Here is the total: ” + total, I had to do ‘Here is the total: ${total},’ which in itself doesn’t look much better than what I would have done but when you start to have a lot of variables you would like to concatenate to one string it does prove to look much better.

ESLint also ended up teaching me about a few things, I was not aware of “type safety” and the benefits of being type safe instead of using the any type. It also taught me about how some return statements are not needed with array functions if you are just doing one action. As someone who is relatively new to Typescript and Javascript the more I can learn the better but trying to learn how to code in Typescript along with adhering to ESLint's standards is a feat in itself.

## Final Thoughts

Overall, my experience using ESLint  has shown me that it is a great resource to use in projects with many collaborators to make sure everyone is adhering to the same coding standards. However, for individual projects, I can’t get behind using it just because of how much longer it takes me to solve basic coding problems. With that being said, I do recommend using ESLint in future collaborative projects with other developers, but in regard to my individual work, I will be taking my own approach and relying on my own coding standards.


