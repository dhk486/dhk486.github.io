---
layout: essay
type: essay
title: "reflect of smart questions draft"
# All dates must be YYYY-MM-DD format!
date: 2024-09-11
published: true
labels:
  - Typescript
summary: "Reflect on Typescript."
---

## Brief self introduction: 
Before writing about reflection of typescript, I am a non-native english speaker and to be honest, I have a desire to study and work in the game development industry as one of my life goals, so I recklessly jumped into the major of computer science. My journey so far has led me to learn Java and C languages in my CS major class. I have started learning Typescript, which is completely new to me. In this essay, I will reflect on how Typescript compares to Java and C, based on my experiences as a beginner. There may be differences from the facts because I am a complete newbie and in the stage of learning Typescript. 

## Comparison Typescript with Java and C:   
According to StackOverflow’s annual survey, JavaScript ranks first in popularity among developers, with 62.3% preferring it. While TypeScript isn’t ranked at the top, it still enjoys a strong preference at 38.5%. So, what makes TypeScript stand out? Java and C are well-known for their strict static typing systems, which enforce rigid type declarations that don’t change. This provides a high level of safety in code but can be challenging for beginners, as I’ve experienced firsthand.

TypeScript offers a middle ground by introducing static typing to JavaScript, a language that is dynamically typed. Unlike Java and C, TypeScript allows for optional typing, giving developers the flexibility to declare variables without specifying types, though they can also enforce strict types when needed. This flexibility is refreshing compared to the strict rules in Java and C, where every variable must be assigned a specific type and remain consistent. For example, In Java, after variables are declared with a specific type, the type can not change.
```ruby
public class Main {
    public static void main(String[] args) {
        int num = 10;
        // num = "text"; // Error: incompatible types
        System.out.println(num);
    }
}

```
In Typescript, we can specify types like Java and C, but we can use 'any' type which offers flexibility.
```ruby
let num: number = 10;
// num = "text"; // Error: Type 'string' is not assignable to type 'number'
console.log(num);

// Flexible typing (like JavaScript)
let flexible: any = 10;
flexible = "text"; // No error
console.log(flexible);

```
For me, the optional typing in TypeScript feels less restrictive and easier to work with, particularly when I’m experimenting with code. However, I also acknowledge that Java and C’s strict typing can be more reliable, especially in large projects where type safety is crucial.

## Conclusion:
So far, learning TypeScript has been a more relaxed experience compared to the rigid structure of Java and C, thanks to its flexibility. I find myself feeling less overwhelmed by syntax and type rules. That said, I’m still in the early stages of learning TypeScript, so it’s difficult to determine whether it is a better language overall. Each language has its strengths, and I believe that mastering a mix of them will help me become a more versatile developer as I continue to pursue my goal of working in game development. 
