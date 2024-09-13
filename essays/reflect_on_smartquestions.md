---
layout: essay
type: essay
title: "Why Smart Questions Lead to Better Answers"
# All dates must be YYYY-MM-DD format!
date: 2024-09-11
published: true
labels:
  - Typescript
  - Smart question
  - stackoverflow
summary: "Reflection on smart questions."
---
<hr>

## Introduction: 

One of the most important communication skills for a software engineer is the ability to ask questions in a "smart" way. Eric Raymond, in his essay How to Ask Questions the Smart Way, outlines several guidelines that help developers ask well-formulated questions, leading to efficient and effective help. This reflection explores two questions from StackOverflow—one that demonstrates a "smart" way of asking questions and another that exemplifies the "not-so-smart" approach. By analyzing these questions and their outcomes, I gained a deeper understanding of the impact smart questions can have on software development.

<hr>

## A Smart Question:   

The user asks: ["How do you explicitly set a new property on window in TypeScript?"](https://stackoverflow.com/questions/12709074/how-do-you-explicitly-set-a-new-property-on-window-in-typescript) They explain they want to add a property to the window object in TypeScript but are getting errors due to TypeScript's strict type system. They provide an example of the error and the code they are working with.

<pre>
 
Question: How do you explicitly set a new property on window in TypeScript?
  
I setup global namespaces for my objects by explicitly setting a property on window.

        window.MyNamespace = window.MyNamespace || {};

TypeScript underlines MyNamespace and complains that:

>The property 'MyNamespace' does not exist on value of type 'window' any"

I can make the code work by declaring MyNamespace as an ambient variable and dropping the window explicitness but I don't want to do that.

        declare var MyNamespace: any;

        MyNamespace = MyNamespace || {};
  
How can I keep window in there and make TypeScript happy?

As a side note I find it especially funny that TypeScript complains since it tells me that window is of type any which by definitely can contain anything.
  
</pre>

The user provides a clear title describing directly the issue they have. They specifically ask about adding a new property to the windows object in Typescript. As Raymond mentioned, the asker describes their clear goal and the problems’s symptoms. They provide context, including an explanation of what they are trying to do and the error message they are receiving. They also include a code snippet, which is a great way to give others the necessary information to reproduce the issue. In addition, the asker presents their question in a respectful manner without demanding an immediate response. This shows the importance of politeness when we want to ask a smart question. 


<hr>

## A Not So Smart Question:

<pre>

Question: Private props return unmodified or losing values within the class inside scope or usage?
So, I have two classes service-class & entity-class with private constructor & static async method, for creating new instance of class. My service-class create & call new entity-class instance and modified it with its properties.

Example | This is NOT NEST.JS code:
        class Service {
          run() {
             const entity = Entity.createNewEntity(args);

             await entity.methodMother();

             const getMyProps1Back = entity.props1();

             // is [ ] empty array, not modified after methodChild
             console.log(getMyProps1Back);

           }
        }    

Each method of my entity is covered with bind decorator from npm: bind-decorator module

        class Entity {
          this.props1! Array<Record<Type>>;
          this.props2 = new Map([]);


          private constructor(someArgs: any) {
            // some stuff
           this.props1 = [];  
          }

          get getProps1() {
            return this.props1;
          }

          static async createNewEntity() {
             const entity = new Entity();
             // blah-blah work here
             return entity;
          }

           @bind
          public async methodMother() {
            this.props1.push({ some: stuff });

            // 

            this.methodChild();
            // method logic
           }

          @bind
          private methodChild() {
           // adding more elements, or overwriting the array
           this.props1 = [test1, test2, test3];
          }
        }
So my questions here are about explaining why context is lost during calling of methodChild within the methodMother and how is my getter return an unmodified array of props1?

## How does it work, and what should I do to avoid it?

Passing an array like argument and returning it back, like this? Or something else, like makign them anonymous?
            
             @bind
              private methodChild(props1 : Array<OfProps1>) {
                 // adding more elements, or overwriting the array
                 props1 = [test1, test2, test3];

                  return arg;
              }      
             
</pre>

If we see this question at StackOverflow, this question got a minus vote, indicating that the question does not show any research effort. The user asks: ["Private props return unmodified or losing values within the class inside scope or usage?"](https://stackoverflow.com/questions/78959669/private-props-return-unmodified-or-losing-values-within-the-class-inside-scope-o). This title is confusing and difficult to understand. It is unclear what the problem is about, as it uses vague phrases like "return unmodified" and "losing values." While the asker provides some code snippets, they don’t explain what the code is supposed to do, how it behaves incorrectly, or what kind of error they’re encountering. The question hasn’t received detailed or helpful answers. One response asks for clarification, which indicates that the original question isn’t clear enough for others to provide a meaningful answer.


<hr>

## Conclusion:

This exercise has highlighted the importance of asking smart questions in software engineering. The question "How do you explicitly set a new property on window in TypeScript?" shows how clarity, focus, and context lead to detailed and helpful responses. In contrast, the vague and unfocused question "Private props return unmodified or losing values..." demonstrates how poor communication results in minimal or unhelpful answers. Smart questions not only respect the time of others but also lead to quicker, more accurate solutions. This comparison has reinforced the importance of clear, concise communication, which I will apply in future interactions with the developer community.

