---
layout: essay
type: essay
title: "What Makes Good Code?"
# All dates mush be YYYY-MM-DD format!
date: 2024-12-02
published: true
labels:
  - Design Patterns
  - Software Engineering
summary: "Reflection on Design Patterns"
---

# **What Makes Good Code?**

As a student majoring in Computer Science, I often think about one question: *What does it take to become a developer who writes good and efficient code?* If you are reading this and are also a beginner developer like me, you might have experienced writing code without any specific plan and just solving problems step by step. While this can work sometimes, it often makes the code harder to read, more error-prone, and less efficient.

When coding without a clear structure, I faced repeated issues, such as debugging the same error multiple times. It made me think: *How can I prevent these problems and write better code?* One way to solve this is to prepare a "blueprint" before starting to code. In programming, we call this **design patterns**.

---

## **What Are Design Patterns?**

Programming is like building a house. Imagine trying to build a skyscraper without a blueprint. Unless you are a genius architect, the building will likely collapse or be very inefficient. Software development is very similar. **Design patterns** in programming are like the blueprints for constructing software systems. They are not perfect solutions for every problem, but they are proven methods to solve common issues in coding.

Design patterns are especially useful in **team projects**. When working with others, having a shared "blueprint" can make it easier to collaborate, reduce repeated mistakes, and organize the workflow. For beginner developers like me, learning design patterns is a way to improve not only my code but also my teamwork.

---

## **My Experience with Design Patterns**

Currently, I am working as the frontend developer for a project called **"Musicians of Manoa"**. The team leader came up the idea, Design of team project below and other members including me added own ideas on to the design. 

<div style="display: flex; justify-content: space-around;">
  <img src="/img/musician_of_manoa.png" alt="Musicians of Manoa Design" width="600px">
</div>

This is a platform for UH Manoa musicians to organize jam sessions, share feedback, and connect with others. Honestly, I didn't actively think about design patterns when working on this project because I am not yet very familiar with them. However, while writing this essay, I realized I might have been using some patterns without knowing.

Our team started the project using a **Next.js template** provided by the class. This template gave us a basic structure and settings, but we customized many parts to fit our project's goals, especially the frontend design and features. Here are some examples of design patterns I noticed in my work:

---

### **1. Component Pattern**

React supports the **Component Pattern**, where the UI is divided into reusable pieces. In our project, we used React components like `Form`, `Card`, `Row`, `Col`, and `Button` to create modular and reusable UI elements. For example:
- The `Card` component was used to display musician profiles.
- The `Form` component allowed users to register or leave feedback.  

Here is an example of how the `Card` component is used in the **"Musicians of Manoa"** project:

```typescript
<Card style={{ backgroundColor: '#ECDFCC' }}>
  <Card.Body>
    <Row>
      <Col md={4}>
        <Card.Img
          src="/neutral_profile_icon.png"
          alt="Profile Image"
          style={{
            height: '200px',
            width: '80%',
            objectFit: 'cover',
            borderRadius: '50%',
          }}
        />
      </Col>
      <Col md={8}>
        <Card.Title>{personalProfile.name}</Card.Title>
        <p><strong>Username: </strong>{personalProfile.username}</p>
        <p><strong>Musical Tastes: </strong>{personalProfile.musicalTastes}</p>
      </Col>
    </Row>
  </Card.Body>
</Card>
```

---

### **2. Observer Pattern**

In the **Observer Pattern**, changes in state automatically update the UI. This pattern is common in React when using hooks like `useState`.  

For example, in our project, I implemented a **review submission feature**:
- I used `useState` to manage the user's input for rating (`rating`) and comment (`comment`).  
- When the user selected a rating or typed a comment, the `setRating` and `setComment` functions updated the state, which automatically refreshed the UI.  

This real-time interaction provided a smoother user experience and made the app feel more dynamic without extra effort to manually update the UI.

```
const [rating, setRating] = useState(0); // User's rating input
const [comment, setComment] = useState(''); // User's comment input

const handleSubmit = (e: React.FormEvent) => {
  e.preventDefault();
  console.log('Submitted Rating:', rating);
  console.log('Submitted Comment:', comment);
  // Add submission logic here, such as sending data to the server
};
```

---

## **What I Learned and Future Plans**

Looking back, I think the Next.js template helped me start the project faster, but I didn't fully understand its structure. Because of this, I didn't intentionally use design patterns while coding. However, writing this essay gave me a chance to reflect on my code and realize the importance of design patterns.

In the future, I want to apply design patterns more intentionally in my projects. For example, I would like to explore more advanced patterns like the **Factory Pattern**, which could help automate repetitive tasks, such as creating multiple reusable components. By doing this, I hope to become a developer who can write better-structured, more efficient code.

Through this project, I learned that design patterns are not just theoretical ideas. They are practical tools that can improve my coding and help me grow as a developer.

---

**Attribution:**  
This essay was written based on my personal experience and understanding. Grammar and formatting assistance were provided using ChatGPT to ensure clarity and correctness.
