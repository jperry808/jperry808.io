---
layout: essay
type: essay
title: "The Scoop on Design Patterns: Scaling with Simplicity"
# All dates must be YYYY-MM-DD format!
date: 2024-12-05
published: true
labels:
  - ICS 314
  - Design Patterns
  - Factory Method
---
You may have noticed that, along your coding journey, you’ve reused ideas or solutions to problems that you encountered early in your coding career. Well, software developers have also noticed this, and they rely on what’s known as a “design pattern.” Design patterns are proven solutions to recurring challenges. To better understand design patterns, you can think of them like using a recipe in cooking. Recipes provide people with a proven way to solve their problems, similar to a design pattern in software engineering. Having these “recipes” or design patterns helps ensure you don’t always have to reinvent the wheel every time you cook (or code).

## Why use design patterns?

Design patterns are important for everyone pursuing software engineering. Not only do they make coding easier for yourself, but they also make it easier for colleagues to understand and debug your code. Design patterns are reliable, proven solutions that can help you solve problems that reoccur in most of your projects.
One of the most reliable methods is the “Factory Method.” The factory method is a design pattern that provides an interface for creating objects in a class. You can then create subclasses under the said class that change the objects to be created. If your project only works with one big class, using the factory method is pointless. But let’s say you wanted to scale your project in the future, and all your code resides in the one class you made. Now, creating another class would result in a lot of redundant and duplicate code. However, if you used the factory method, scaling your project and adding a new class would be extremely simple! Let’s look at an example.

## Factory Method Example

<div style="display: flex; align-items: flex-start; flex-wrap: wrap; gap: 10px;">
  <div style="flex: 1; min-width: 300px; max-width: 50%;">
    <img src="https://i.pinimg.com/736x/60/c4/d1/60c4d150b4b4a2bf4f7f32cbfa8acfe0.jpg" style="width: 100%; border: 1px solid #ddd; border-radius: 5px;">
  </div>
  <div style="flex: 2; min-width: 300px;">

Let’s think of a food ordering app, maybe an ice cream ordering app. Initially, your ice cream shop opens up offering only vanilla ice cream. All your code for ordering ice cream resides in the “Vanilla” class. You then realize that nobody wants vanilla ice cream anymore, so you need to add new flavors before you go out of business! Since all your code is in the “Vanilla” class, adding new flavors would be a lot of work and require a lot of duplicate code. You then think back to your software engineering class and remember the factory method! Instead of a “Vanilla” class, we create an “IceCream” interface that each ice cream flavor class can implement. Here is a quick example in code:

```typescript
// IceCream.tsx
export interface IceCream { 
   scoop(): void;
}

// Vanilla.tsx
import { IceCream } from './IceCream';

export class Vanilla implements IceCream {
   scoop() {
      console.log("Ordering a scoop of vanilla ice cream!");
   }
}

// MintChocolateChip.tsx
import { IceCream } from './IceCream';

export class MintChocolateChip implements IceCream {
   scoop() {
      console.log("Ordering a scoop of mint chocolate chip ice cream!");
   }
}
```

Now, creating new flavors is super simple, and your code is scalable for the future of your ice cream business. None of the classes you just created need to be updated if you want to add a new flavor—just your main function or a separate function that handles ice cream class creation.

  </div>
</div>

## Final Thoughts

There are so many different design patterns out there, and they are all beneficial in certain situations. The situation I covered with the factory method is a very common one and is one I have used myself in various coding projects during my college career. Understanding these concepts is a necessary stepping stone for any aspiring software engineer. Whether you’re creating an ice cream shop app or building a large-scale system, design patterns are a cornerstone of effective software development.



